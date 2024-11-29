# Bibliotecas_pandas-seaborn-matplotlib-plotly-cufflinks-chart_studio-scikit-learn

# Previsão de Preços de Imóveis nos EUA

Este projeto utiliza um modelo de regressão linear para prever os preços de imóveis nos EUA com base em diversas características, como renda média da área, idade média da casa e tamanho da população.

**Bibliotecas:**

- **pandas:** Para manipulação e análise de dados.
- **seaborn:** Para visualização de dados estatísticos.
- **matplotlib:** Para criação de gráficos estáticos, como gráficos de dispersão e histogramas.
- **plotly:** Para criação de gráficos interativos.
- **cufflinks:** Para conectar o pandas e o plotly, permitindo a criação de gráficos interativos diretamente de DataFrames do pandas.
- **chart-studio:** Para publicar gráficos do plotly online.
- **scikit-learn:** Para aprendizado de máquina, incluindo a classe `LinearRegression` para regressão linear.
- **numpy:** Para operações numéricas eficientes em arrays multidimensionais.

## Descrição do Código

O código realiza as seguintes etapas:

1. **Carregamento dos Dados:**
   - Importa a biblioteca pandas e carrega os dados do arquivo "USA_Housing.csv" para um DataFrame.
   - Arredonda os valores numéricos para duas casas decimais.
   - Exibe as primeiras linhas do DataFrame para inspeção inicial.

2. **Exploração dos Dados:**
   - Usa o método `info()` para exibir informações sobre o DataFrame, como número de linhas, colunas, tipos de dados e uso de memória.
   - Usa o método `describe()` para obter estatísticas descritivas dos dados numéricos, como média, desvio padrão, mínimo, máximo e quartis.
   - Cria box plots para visualizar a distribuição da renda média da área e do preço do imóvel.
   - Renomeia colunas para facilitar a manipulação.
   - Remove a coluna "Address" do DataFrame.
   - Cria um pair plot para visualizar as relações entre todas as colunas numéricas.
   - Cria um pair plot para visualizar as relações entre as variáveis independentes (features) e a variável dependente (preço do imóvel).
   - Calcula a matriz de correlação entre as colunas numéricas.
   - Cria um heatmap da matriz de correlação para visualizar as relações entre as variáveis.
   - Cria um histograma para visualizar a distribuição do preço do imóvel.

3. **Preparação dos Dados:**
   - Define as variáveis independentes (X) e a variável dependente (Y).
   - Divide os dados em conjuntos de treinamento e teste usando a função `train_test_split` da biblioteca scikit-learn.
   - Exibe as dimensões dos conjuntos de dados de treinamento e teste.

4. **Criação e Treinamento do Modelo:**
   - Importa a classe `LinearRegression` da biblioteca scikit-learn.
   - Cria um objeto do modelo de regressão linear.
   - Treina o modelo usando os dados de treinamento.

5. **Avaliação do Modelo:**
   - Faz previsões sobre os dados de teste usando o modelo treinado.
   - Calcula o R² (coeficiente de determinação) para avaliar o desempenho do modelo.
   - Exibe o valor do R².

6. **Visualização dos Resultados:**
   - Cria um gráfico de dispersão para comparar os valores reais e os valores previstos.

7. **Previsão com Novos Dados:**
   - Cria dados de entrada para uma nova previsão.
   - Faz uma previsão usando o modelo treinado e os novos dados de entrada.
