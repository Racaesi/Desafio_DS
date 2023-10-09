# Desafio Data Science - Lighthouse

## O problema

O desafio tem como objetivo avaliar o desenvolvimento de uma EDA (exploratory data analysis) e os conhecimentos/insights relacionados a séries temporais. Para isso, este desafio abordará a previsão de crescimento do índice GDP de cada país nos anos de 2024-2028.

### Informações sobre os dados:

- Os valores numéricos de GDP são valores percentuais.
- O dataset apresenta valores preenchidos como 'no data'.
- O próprio dataset ja traś valores de GDP para 2024 a 2028, resultados de uma previsão de série temporal cujo método é desconhecido.

## Primeiros passos para solução do problema

### 1) Análise do dataset

Entender como os valores 'no data' estão distribuídos para os países, substitui-los por 'None' e verificar o percentual que os valores nulos representam para cada país.

Foi verificado que o dataset também contém os valors de GPD para grupos/categorias, dividos em: economias, regiões, continentes e conjunto de continentes.

### 2) Países por grupo/categoria

Foram criadas diversas listas com os mesmos nomes dos grupos e categorias já existentes e, definido quais paises portenceriam a eles. Dessa forma, foi realizada uma análise gráfica dos dados considerados do passado (1980 até 2023) e verificado se haveria alguma semelhança nas curvas desses paises. 

A partir desse momento, foram análisados todos os paises que apresentavam dados faltantes e definido quais os grupos que seriam utilizados para susbtituição dos valores nulos. 

#### a) Os seguintes grupos foram utilizados para substituir os valores nulos dos paises:

- South Asia
- Advanced Economies
- Africa
- Europe
- Middle East
- Pacific Islands
- Southeast Asia
- Central America

#### b) Os seguintes grupos foram utilizados para substituir os valores nulos dos próprios grupos:

- Sub-Saharan Africa (Region)
- Sub-Saharan Africa
- Euro area
- Middle East
- Central Asia and the Caucasus
- Central America

### 3) Definição do método para substituição dos valores nulos

## 4) Escolha do modelo final


## 5) Executando o projeto

### 5.1) Clonar o repositório

` git clone https://github.com/Racaesi/desafio_ds_lighthouse.git` 

### 6.2) Criação do ambiente virtual

`python -m venv venv` 

### 6.3) Ativar a venv no linux

`source venv/bin/activate`

### 6.4) Instalar as dependências

`pip install -r requirements.txt`

### 6.5) Executar o notebook

Este notebook gera apenas um arquivo de saída 'df_predictions.csv' com o modelo final de predição. 