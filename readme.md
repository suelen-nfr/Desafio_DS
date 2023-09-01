# Desafio de Data Science
O desafio tem como objetivo desenvolver um EDA (exploratory data analysis) e os conhecimentos/insights relacionados a um tipo clássico de problema de data science: séries temporais. Para isso, foi previsto o crescimento do índice GDP de cada país nos anos de 2024-2028, sendo compadaro posteriormente com o previsto pelo Statistica

## Começando
O desafio foi desenvolvido com o Google Colab, seguindo a seguinte estrutura:

## Pré-requisitos
Os pacotes necessários constam no arquivo requirements.txt

## Instalação
Instalando e ativando a venv:
    !sudo apt install python3.10-venv
    !python3 -m venv venv
    !source venv/bin/activate

Instalando os requirements:
    !pip install -r requirements.txt

Instalando as bibliotecas e pacotes necessários:
    !pip install statsforecast
    !pip install datasetsforecast

    from google.colab import drive
    drive.mount ('/content/drive')

    import pandas as pd
    import numpy as np
    import seaborn as sns
    import matplotlib.pyplot as plt
    import matplotlib as mpl

    from statsforecast import StatsForecast
    from statsforecast.models import (
    AutoARIMA,
    HoltWinters,
    CrostonClassic as Croston,
    HistoricAverage,
    DynamicOptimizedTheta as DOT,
    SeasonalNaive
    )
    from datasetsforecast.losses import mse, mae, rmse

## Acessando os dados raw
Para o Eda:
df = pd.read_excel('/content/drive/MyDrive/Lighthouse/Desafio DS/imf-dm-export-20230513.xlsx')
df.head()

Para a modelagem e predição;
df = pd.read_excel('/content/drive/MyDrive/Lighthouse/Desafio DS/EDA_desafioDS.xlsx')
df.head()

## Ferramentas utilizadas
Google Colab
StatsForecast
Pandas
Matplotlib
Plotly

## Fontes
https://nixtla.github.io/statsforecast/
https://www.imf.org/en/Publications/WEO/weo-database/2023/April/select-aggr-data

## Autores
Suelen Nobre Franco Rodrigues

## Expressões de gratidão
Imensa gratidão à Indicium por nos proporcionar essa oportunidade única
e aos colegas de Lighthouse por todo apoio.