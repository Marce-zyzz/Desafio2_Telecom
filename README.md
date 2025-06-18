# Desafio2_Telecom
Descripción del Proyecto
Telecom X enfrenta una alta tasa de cancelaciones de clientes (churn) que afecta su rentabilidad y crecimiento. Como parte del equipo de Data Science, este proyecto tiene como objetivo analizar los datos históricos de clientes para identificar patrones y factores que contribuyen a la evasión.

El análisis permitirá obtener información valiosa que facilitará la creación de modelos predictivos y el desarrollo de estrategias orientadas a retener clientes y reducir la tasa de cancelación.
Objetivos
Cargar y limpiar los datos de clientes y sus servicios.

Explorar las variables relevantes, tanto categóricas como numéricas.

Visualizar las distribuciones y relaciones entre variables.

Calcular medidas de asociación entre variables categóricas y numéricas.

Identificar características clave que se relacionan con la evasión.

Proporcionar insights para el desarrollo posterior de modelos predictivos.
Descripción de los Datos
Los datos provienen de un archivo JSON con la información de clientes, que incluye:

Datos personales (customer)

Información de teléfono (phone)

Servicios de internet contratados (internet)

Datos de cuenta (account)

Cada sección contiene variables específicas que serán normalizadas y unificadas en un único DataFrame para facilitar el análisis.

ecnologías y Herramientas Utilizadas
Python 3.8+

Pandas

NumPy

Matplotlib

Seaborn

SciPy
Estructura del Código
1. Carga y limpieza de datos
Descarga de datos JSON desde URL.

Normalización de datos anidados.

Limpieza y transformación de variables clave (Churn, SeniorCitizen, etc.).

Eliminación de columnas irrelevantes.

2. Análisis exploratorio de datos (EDA)
Visualización de distribuciones para variables categóricas.

Análisis de variables numéricas con respecto a la evasión (Churn).

Cálculo de correlaciones para variables numéricas.

Uso del coeficiente V de Cramer para medir asociación entre variables categóricas.

3. Visualizaciones
Gráficos de barras con seaborn.countplot para variables categóricas.

Diagramas de caja (boxplots) para variables numéricas vs. Churn.

Mapas de calor (heatmaps) para correlaciones.

Funciones Principales
load_and_clean_data_json(url): Carga datos desde JSON anidado, normaliza y limpia el DataFrame.

cramers_v(x, y): Calcula el coeficiente V de Cramer para medir asociación entre variables categóricas.

plot_distributions(df, columns, hue): Visualiza distribuciones de variables categóricas.

plot_numerical_vs_churn(df, num_cols): Boxplots para variables numéricas frente a la variable objetivo Churn.

plot_correlations(df, num_cols, cat_cols): Visualiza mapas de calor con correlaciones numéricas y categóricas.

Resultados Esperados
Identificación de variables con mayor influencia en la evasión.

Visualizaciones claras que ayuden a interpretar los factores clave.

Base sólida para implementar modelos de machine learning que predigan el churn.

Insights accionables para diseñar estrategias de retención de clientes.
