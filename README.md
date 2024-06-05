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
````

## Como Executar no Google Colab
1. Abra o Google Colab em seu navegador.
2. Faça login com sua conta do Google.
3. Clique em "Arquivo" -> "Abrir notebook".
4. Na guia "GitHub", cole o link do repositório: `https://github.com/seu_usuario/imigracao-america-sul-canada`.
5. Selecione o notebook principal ou o script de análise (`analise_imigracao.ipynb` ou `analise_imigracao.py`).
6. Clique em "Abrir".
7. Execute as células do notebook para reproduzir a análise.

## Dependências
- Python 3.8+
- Plotly
- Pandas

## Agradecimentos
Agradeço à Alura pelo excelente curso e à comunidade de Data Science pelo suporte contínuo.

## Contato
Para mais informações, entre em contato:

Email: helviley.melo@gmail.com
LinkedIn: linkedin.com/in/helviley-lacerda-2253a2115/

