# Análise de Imigração da América do Sul para o Canadá (1980-2013)

![Plotly](https://img.shields.io/badge/Plotly-Interactive%20Plots-blue)
![Python](https://img.shields.io/badge/Python-3.8%2B-green)
![Alura](https://img.shields.io/badge/Alura-Data%20Science-orange)

## Descrição
Este repositório contém a análise de imigração dos países da América do Sul para o Canadá entre 1980 e 2013. Utilizando Python e a biblioteca Plotly, foram criadas visualizações interativas para melhor compreensão dos dados migratórios.

## Projeto
Durante o curso **Data Science: Explorando e Analisando Dados** pela plataforma Alura, desenvolvi um projeto para analisar os dados de imigração e criar visualizações interativas. O gráfico abaixo ilustra a imigração de diferentes países sul-americanos para o Canadá ao longo dos anos.

## Visualização Interativa
```python
import plotly.express as px

fig = px.line(america_sul_final, x=america_sul_final.index, y=america_sul_final.columns, color='País',
              title='Imigração dos países da América do Sul para o Canadá no período de 1980 a 2013', markers=True)
fig.update_layout(width=1000, height=500, xaxis={'tickangle':-45},
                  font_family='Arial',
                  font_size=14,
                  font_color='grey',
                  title_font_color='black',
                  title_font_size=22,
                  xaxis_title='Ano',
                  yaxis_title='Número de imigrantes')
fig.show()


