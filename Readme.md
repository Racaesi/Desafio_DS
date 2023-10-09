# Desafio Data Science - Lighthouse

## O problema

O desafio tem como objetivo avaliar o desenvolvimento de uma EDA (exploratory data analysis) e os conhecimentos/insights relacionados a séries temporais. Para isso, este desafio abordará a previsão de crescimento do índice GDP de cada país nos anos de 2024-2028.

### Informações sobre os dados:

- Os valores numéricos de GDP são valores percentuais.
- O dataset apresenta valores preenchidos como 'no data'.
- O próprio dataset ja traś valores de GDP para 2024 a 2028, resultados de uma previsão de série temporal cujo método é desconhecido.

## Primeiros passos para solução do problema

### 1) Análise do dataset

Entender como os valores 'no data' estão distribuídos para os países.

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

### 3) Validando os dados tratados/pré-processados e salvando num arquivo .csv
A partir desse momento, foi gerado um arquivo csv com dados pré-processados que podem ser utilizados para o modelo de predição que mais for performático.
Optou-se por essa decisão, para facilitar o processo de feature engeneering, sem precisar revisitar os passos de EDA.
Nesse caso então ainda haverão dados `NaN` para tratativas.
 
### 4) Escolha do modelo final

### 5) Executando o projeto

### 6) Executar o notebook

Este notebook gera alguns arquivos de saída:
* 'df_eda.csv' com dados pré-processados
* 'df_predictions.csv' com o modelo final de predição. 