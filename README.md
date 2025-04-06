# 📊 Predictive Analysis with AdaBoost: Lead Conversion and Medical Costs

This project uses Machine Learning techniques with the **AdaBoost** algorithm to build classification and regression models. The goal is to predict:

- Whether a lead will convert or not (classification)
- The estimated medical cost of a patient (regression)

## 🧰 Technologies and Libraries

- Python
- Pandas, NumPy
- Seaborn, Matplotlib, Plotly
- Scikit-learn
- Joblib

## 📁 Data Structure

### 1. Leads (`leads_cleaned.csv`)

- Dataset with information about sales leads.
- Target variable: `Converted` (1 = converted, 0 = not converted)

### 2. Medical Costs (`healthcosts_cleaned.csv`)

- Dataset with demographic and health habit data of patients.
- Target variable: `medical charges` (medical cost amount)

## 🔍 Project Steps

### 1. Exploratory Data Analysis (EDA)

- Viewing the first/last rows of the datasets
- Checking data types and structure

### 2. Preprocessing

- Splitting into predictor variables (`X`) and target variable (`y`)
- Transformations with `ColumnTransformer` including:
  - `StandardScaler` for numerical variables
  - `OneHotEncoder` for categorical variables
- Use of `joblib` to save and load the preprocessor

### 3. Model Training

#### Classification (Leads)

- Algorithm: `AdaBoostClassifier` with `LogisticRegression` as base estimator
- Metrics:
  - Accuracy, Precision, Recall, F1 Score
  - Confusion Matrix using `Plotly`
- Feature importance analysis

#### Regression (Medical Costs)

- Algorithm: `AdaBoostRegressor` with `LinearRegression` as base estimator
- Metrics:
  - R² (Coefficient of Determination)
  - RMSE (Root Mean Squared Error)
- Visualization of feature importance

### 4. Results and Interpretation

- Interactive visualization of confusion matrix and feature importance
- Access to estimator errors and weights
- Probability predictions with the classification model

## 📦 Generated Files

- `preprocessor_dataset_leads.pkl`: Preprocessing pipeline for leads dataset
- `preprocessor_dataset_healthcosts.pkl`: Preprocessing pipeline for health dataset
- `leads_cleaned.csv`: Cleaned version of leads data
- `healthcosts_cleaned.csv`: Cleaned version of health data

## 📈 Visualizations

- Feature importance using bar charts
- Interactive confusion matrix with Plotly

## 🧠 Requirements to Run the Project

Install the required packages with:

```bash
pipenv install pandas numpy matplotlib seaborn plotly nbformat scipy scikit-learn ipykernel
```

Or, if using `pip`:

```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn joblib
```

## 🚀 How to Run

1. Clone the repository and open the notebooks or `.py` scripts.
2. Make sure the `.csv` and `.pkl` files are in the `datasets/` folder.
3. Execute the code blocks sequentially.
4. The results will be displayed directly in the interactive interface (Jupyter or VSCode).

---

# 📊 Análisis Predictivo con AdaBoost: Conversión de Leads y Costos Médicos

Este proyecto utiliza técnicas de Machine Learning con el algoritmo **AdaBoost** para construir modelos de clasificación y regresión. El objetivo es predecir:

- Si un lead se convertirá o no (clasificación)
- El costo médico estimado de un paciente (regresión)

## 🧰 Tecnologías y Bibliotecas

- Python
- Pandas, NumPy
- Seaborn, Matplotlib, Plotly
- Scikit-learn
- Joblib

## 📁 Estructura de los Datos

### 1. Leads (`leads_cleaned.csv`)

- Conjunto de datos con información sobre leads de ventas.
- Variable objetivo: `Converted` (1 = convertido, 0 = no convertido)

### 2. Costos Médicos (`healthcosts_cleaned.csv`)

- Conjunto de datos con información demográfica y hábitos de salud de los pacientes.
- Variable objetivo: `medical charges` (monto del costo médico)

## 🔍 Etapas del Proyecto

### 1. Análisis Exploratorio de Datos (EDA)

- Visualización de las primeras/últimas filas del conjunto de datos
- Verificación de tipos de datos y estructura

### 2. Preprocesamiento

- División entre variables predictoras (`X`) y variable objetivo (`y`)
- Transformaciones con `ColumnTransformer` que incluyen:
  - `StandardScaler` para variables numéricas
  - `OneHotEncoder` para variables categóricas
- Uso de `joblib` para guardar y cargar el preprocesador

### 3. Entrenamiento del Modelo

#### Clasificación (Leads)

- Algoritmo: `AdaBoostClassifier` con `LogisticRegression` como estimador base
- Métricas:
  - Precisión, Exactitud, Recall, F1 Score
  - Matriz de Confusión usando `Plotly`
- Análisis de importancia de las características

#### Regresión (Costos Médicos)

- Algoritmo: `AdaBoostRegressor` con `LinearRegression` como estimador base
- Métricas:
  - R² (Coeficiente de Determinación)
  - RMSE (Raíz del Error Cuadrático Medio)
- Visualización de la importancia de las variables

### 4. Resultados e Interpretación

- Visualización interactiva de la matriz de confusión e importancia de las variables
- Acceso a errores y pesos de los estimadores
- Predicción de probabilidades en el modelo de clasificación

## 📦 Archivos Generados

- `preprocessor_dataset_leads.pkl`: Pipeline de preprocesamiento para el conjunto de datos de leads
- `preprocessor_dataset_healthcosts.pkl`: Pipeline de preprocesamiento para el conjunto de datos de salud
- `leads_cleaned.csv`: Versión limpia de los datos de leads
- `healthcosts_cleaned.csv`: Versión limpia de los datos de salud

## 📈 Visualizaciones

- Importancia de las características usando gráficos de barras
- Matriz de confusión interactiva con Plotly

## 🧠 Requisitos para Ejecutar el Proyecto

Instala los paquetes necesarios con:

```bash
pipenv install pandas numpy matplotlib seaborn plotly nbformat scipy scikit-learn ipykernel
```

O, si usas `pip`:

```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn joblib
```

## 🚀 Cómo Ejecutar

1. Clona el repositorio y abre los notebooks o scripts `.py`.
2. Asegúrate de que los archivos `.csv` y `.pkl` estén en la carpeta `datasets/`.
3. Ejecuta los bloques de código secuencialmente.
4. Los resultados se mostrarán directamente en la interfaz interactiva (Jupyter o VSCode).

---

# 📊 Análise Preditiva com AdaBoost: Conversão de Leads e Custos Médicos

Este projeto utiliza técnicas de Machine Learning com o algoritmo **AdaBoost** para construir modelos de classificação e regressão. O objetivo é prever:

- Se um lead será convertido ou não (classificação)
- O custo médico estimado de um paciente (regressão)

## 🧰 Tecnologias e Bibliotecas

- Python
- Pandas, NumPy
- Seaborn, Matplotlib, Plotly
- Scikit-learn
- Joblib

## 📁 Estrutura dos Dados

### 1. Leads (`leads_cleaned.csv`)

- Base de dados com informações sobre leads de vendas.
- Variável alvo: `Converted` (1 = convertido, 0 = não convertido)

### 2. Custos Médicos (`healthcosts_cleaned.csv`)

- Base com dados demográficos e hábitos de saúde dos pacientes.
- Variável alvo: `medical charges` (valor do custo médico)

## 🔍 Etapas do Projeto

### 1. Análise Exploratória (EDA)

- Visualização das primeiras/últimas linhas dos dados
- Verificação de tipos e estrutura

### 2. Pré-processamento

- Divisão em variáveis preditoras (`X`) e variável alvo (`y`)
- Transformações com `ColumnTransformer` contendo:
  - `StandardScaler` para variáveis numéricas
  - `OneHotEncoder` para variáveis categóricas
- Uso de `joblib` para salvar e carregar o preprocessor

### 3. Treinamento de Modelos

#### Classificação (Leads)

- Algoritmo: `AdaBoostClassifier` com `LogisticRegression` como base
- Métricas:
  - Acurácia, Precisão, Recall, F1 Score
  - Matriz de Confusão com `Plotly`
- Análise de importância das features

#### Regressão (Custos Médicos)

- Algoritmo: `AdaBoostRegressor` com `LinearRegression` como base
- Métricas:
  - R² (Coeficiente de Determinação)
  - RMSE (Erro Quadrático Médio)
- Visualização da importância das variáveis

### 4. Resultados e Interpretação

- Visualização interativa da matriz de confusão e importância das variáveis
- Acesso aos erros e pesos dos estimadores
- Predição de probabilidades no modelo de classificação

## 📦 Arquivos Gerados

- `preprocessor_dataset_leads.pkl`: Pipeline de pré-processamento dos dados de leads
- `preprocessor_dataset_healthcosts.pkl`: Pipeline de pré-processamento dos dados de saúde
- `leads_cleaned.csv`: Versão limpa dos dados de leads
- `healthcosts_cleaned.csv`: Versão limpa dos dados de saúde

## 📈 Visualizações

- Importância das features usando gráficos de barras
- Matriz de confusão interativa com Plotly

## 🧠 Requisitos para Rodar o Projeto

Instale os pacotes necessários com:

```bash
pipenv install pandas numpy matplotlib seaborn plotly nbformat scipy scikit-learn ipykernel
```

Ou, se estiver usando `pip`:

```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn joblib
```

## 🚀 Como Rodar

1. Clone o repositório e abra os notebooks ou scripts `.py`.
2. Certifique-se de que os arquivos `.csv` e `.pkl` estejam na pasta `datasets/`.
3. Execute os blocos de código sequencialmente.
4. Os resultados serão exibidos diretamente na interface interativa (Jupyter ou VSCode).
