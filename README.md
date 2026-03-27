# telecom-analysis

📊 Análisis de Uso de Clientes – ConnectaTel
🎯 Objetivo del proyecto

El objetivo de este proyecto es analizar el comportamiento de uso de los clientes de ConnectaTel, identificando patrones de consumo, segmentando usuarios según su nivel de uso y generando insights accionables que apoyen la toma de decisiones de negocio, especialmente en la optimización de planes y estrategias comerciales.

🗂️ Datasets utilizados

Se utilizaron tres datasets:
1. plans
Información de los planes ofrecidos por la compañía
Variables típicas: plan, precio, minutos_incluidos, mensajes_incluidos
Permite analizar la relación entre consumo y oferta comercial
2. users
Información de los clientes
Variables relevantes: user_id, age, city, plan, reg_date
3. usage
Registro de uso del servicio
Variables relevantes: user_id, type (call/text), duration, length, date

🔎 Etapas del análisis

El análisis se desarrolló en las siguientes etapas:

1. Exploración de datos (EDA)
Revisión de tipos de datos
Análisis de valores únicos y distribución
Identificación de inconsistencias
2. Limpieza de datos
Tratamiento de valores nulos (estructurales vs reales)
Identificación y manejo de fechas inconsistentes
Validación de variables numéricas
3. Transformación de datos
Creación de variables agregadas por usuario:
cant_mensajes
cant_llamadas
cant_minutos_llamada
Unión de datasets (usage + users)
4. Análisis exploratorio
Distribución de variables (histogramas)
Comparación por tipo de plan
Identificación de outliers (boxplots + IQR)
5. Segmentación de clientes
Clasificación en:
Bajo uso
Uso medio
Alto uso
6. Generación de insights
Identificación de usuarios intensivos (heavy users)
Evaluación del valor de segmentos
Recomendaciones de negocio

▶️ Cómo ejecutar el notebook

Puedes ejecutar este proyecto de las siguientes formas:

🔹 Google Colab
Abre Google Colab: https://colab.research.google.com/
Sube el archivo .ipynb
Ejecuta las celdas en orden
🔹 Opción 2: Jupyter Notebook (local)

Clona este repositorio:

git clone <URL_DEL_REPOSITORIO>

Instala dependencias:

pip install pandas numpy matplotlib seaborn

Ejecuta:

jupyter notebook
