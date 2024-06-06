# Análise Preditiva de Doenças Cardíacas: Relatório Técnico

## 1. Coleta de Dados

O dataset utilizado neste projeto, `doencacoracao.csv`, contém informações médicas relevantes para a predição de doenças cardíacas. As variáveis presentes no conjunto de dados incluem:

* **Variáveis Demográficas:**
    * Idade (Age)
    * Sexo (Sex)
* **Histórico Médico:**
    * Tipo de dor no peito (Chest pain type)
    * Pressão arterial (BP)
    * Nível de colesterol (Cholesterol)
    * Diabetes (FBS over 120)
* **Resultados de Exames:**
    * Resultados de eletrocardiograma (EKG results)
    * Frequência cardíaca máxima (Max HR)
    * Angina induzida por exercício (Exercise angina)
    * Depressão do segmento ST (ST depression)
    * Inclinação do segmento ST (Slope of ST)
    * Número de vasos sanguíneos com obstrução (Number of vessels fluro)
    * Resultados do teste de tálio (Thallium)
* **Variável Alvo:**
    * Presença ou ausência de doença cardíaca (Heart Disease)

## 2. Modelagem

### Pré-processamento dos Dados

* **Codificação de Rótulos (Label Encoding):** Variáveis categóricas foram convertidas em valores numéricos.
* **Padronização (StandardScaler):** Variáveis numéricas foram padronizadas (média zero, desvio padrão um).

### Divisão dos Dados

* **Treinamento (80%):** Dados usados para treinar os modelos.
* **Teste (20%):** Dados usados para avaliar os modelos.

### Treinamento e Avaliação dos Modelos

Diversos modelos de classificação foram treinados e avaliados, utilizando a acurácia como métrica:

* Regressão Logística
* K-Nearest Neighbors (KNN)
* Support Vector Machines (SVM)
* Árvores de Decisão
* Random Forest
* Gradient Boosting
* AdaBoost
* Naive Bayes
* XGBoost

### Seleção do Melhor Modelo

O modelo de **Regressão Logística** obteve a maior acurácia (92.5%) e foi selecionado.

### Avaliação Detalhada do Modelo Escolhido

A matriz de confusão foi utilizada para analisar o desempenho do modelo de Regressão Logística, revelando os verdadeiros positivos, verdadeiros negativos, falsos positivos e falsos negativos.

## 3. Conclusões

* A análise exploratória forneceu insights valiosos sobre as variáveis e suas relações com a doença cardíaca.
* O modelo de Regressão Logística demonstrou ser eficaz na previsão da doença cardíaca, com alta acurácia.
* A matriz de confusão confirmou o bom desempenho do modelo tanto na identificação de pacientes com doença cardíaca quanto na identificação de pacientes sem a doença.
