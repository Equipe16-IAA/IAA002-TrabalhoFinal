# IAA002-TrabalhoFinal

Trabalho final da disciplina de Linguagem de Programação Aplicada

---
Nome da base de dados do exercício: precos_carros_brasil.csv
Informações sobre a base de dados:
Dados dos preços médios dos carros brasileiros, das mais diversas marcas, no ano de 2021, de acordo com dados extraídos da tabela FIPE (Fundação Instituto de Pesquisas Econômicas). A base original foi extraída do site Kaggle [Acesse aqui a base original](https://www.kaggle.com/datasets/vagnerbessa/average-car-prices-bazil/data). A mesma foi adaptada para ser utilizada no presente exercício.

Observação: As variáveis fuel, gear e engine_size foram extraídas dos valores da coluna model, pois na base de dados original não há coluna dedicada a esses valores. Como alguns valores do modelo não contêm as informações do tamanho do motor, este conjunto de dados não contém todos os dados originais da tabela FIPE.

**Metadados:**

Nome do campo |Descrição
--------------|----------
year_of_reference |O preço médio corresponde a um mês de ano de referência
month_of_reference |O preço médio corresponde a um mês de referência, ou seja, a FIPE atualiza sua tabela mensalmente
fipe_code |Código único da FIPE
authentication |Código de autenticação único para consulta no site da FIPE
brand |Marca do carro
model |Modelo do carro
fuel |Tipo de combustível do carro
gear |Tipo de engrenagem do carro
engine_size |Tamanho do motor em centímetros cúbicos
year_model |Ano do modelo do carro. Pode não corresponder ao ano de fabricação
avg_price |Preço médio do carro, em reais

**Atenção: ao fazer o download da base de dados, selecione o formato .csv. É o formato que será considerado correto na resolução do exercício.**

---

### 1. Análise Exploratória dos dados

A partir da base de dados precos_carros_brasil.csv, execute as seguintes tarefas:

  a. Carregue a base de dados media_precos_carros_brasil.csv
  
  b. Verifique se há valores faltantes nos dados. Caso haja, escolha uma tratativa para resolver o problema de valores faltantes
  
  c. Verifique se há dados duplicados nos dados
  
  d. Crie duas categorias, para separar colunas numéricas e categóricas. Imprima o resumo de informações das variáveis numéricas e categóricas (estatística descritiva dos dados)
  
  e. Imprima a contagem de valores por modelo (model) e marca do carro (brand)
  
  f. Dê um breve explicação (máximo de quatro linhas) sobre os principais resultados encontrados na Análise Exploratória dos dados

---

  ### 2. Visualização dos dados
  
A partir da base de dados precos_carros_brasil.csv, execute as seguintes tarefas:

a. Gere um gráfico da distribuição da quantidade de carros por marca

b. Gere um gráfico da distribuição da quantidade de carros por tipo de engrenagem do carro

c. Gere um gráfico da evolução da média de preço dos carros ao longo dos meses de 2022 (variável de tempo no eixo X)

d. Gere um gráfico da distribuição da média de preço dos carros por marca e tipo de engrenagem

e. Dê uma breve explicação (máximo de quatro linhas) sobre os resultados gerados no item d

f. Gere um gráfico da distribuição da média de preço dos carros por marca e tipo de combustível

g. Dê uma breve explicação (máximo de quatro linhas) sobre os resultados gerados no item f

---

### 3. Aplicação de modelos de machine learning para prever o preço médio dos carros

A partir da base de dados precos_carros_brasil.csv, execute as seguintes tarefas:

a. Escolha as variáveis numéricas (modelos de Regressão) para serem as variáveis independentes do modelo.A variável target é avg_price. Observação: caso julgue necessário, faça a transformação de variáveis categóricas em variáveis numéricas para inputar no modelo. Indique quais variáveis foram transformadas e como foram transformadas

b. Crie partições contendo 75% dos dados para treino e 25% para teste

c. Treine modelos RandomForest (biblioteca RandomForestRegressor) e XGBoost (biblioteca XGBRegressor) para predição dos preços dos carros. Observação: caso julgue necessário, mude os parâmetros dos modelos e rode novos modelos. Indique quais parâmetros foram inputados e indique o treinamento de cada modelo

d. Grave os valores preditos em variáveis criadas

e. Realize a análise de importância das variáveis para estimar a variável target, para cada modelo treinado

f. Dê uma breve explicação (máximo de quatro linhas) sobre os resultados encontrados na análise de importância de variáveis

g. Escolha o melhor modelo com base nas métricas de avaliação MSE, MAE e R²

h. Dê uma breve explicação (máximo de quatro linhas) sobre qual modelo gerou o melhor resultado e a métrica de avaliação utilizada

  
