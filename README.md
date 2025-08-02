# 📉 Análisis de la Pérdida de Clientes (Churn) y Optimización de Costos

## 📝 Descripción del Proyecto
Este proyecto aborda el desafío de la pérdida de clientes (Churn) en una empresa de telecomunicaciones. El objetivo principal es desarrollar un modelo predictivo para identificar a los clientes en riesgo de abandono y, a partir de este análisis, generar insights accionables para el área financiera (CFO) que permitan optimizar costes y mitigar pérdidas económicas.

El análisis combina técnicas de Machine Learning con un enfoque en la interpretación de los resultados para la toma de decisiones estratégicas.

## 📊 Hallazgos y Recomendaciones Estratégicas
El análisis del modelo ha revelado puntos clave que son críticos para la estrategia de negocio:

- Alto Potencial de Detección: El modelo tiene una alta precisión (86% de ROC AUC) para diferenciar entre clientes que se irán y los que se quedarán. Esto lo convierte en una herramienta sólida para la detección temprana.

- Área de Mejora Crítica (Recall): A pesar de su precisión, el modelo solo identifica al 50% de los clientes que realmente abandonan. Es crucial mejorar este aspecto para evitar que la mitad de las pérdidas de clientes no sean anticipadas.

A partir de estos resultados, se proponen las siguientes recomendaciones estratégicas para reducir el churn y optimizar costes:

1. Fidelización a Largo Plazo: Incentivar a los clientes a migrar de contratos mensuales a anuales mediante descuentos y beneficios exclusivos.

2. Campañas de Seguridad: Reforzar la lealtad ofreciendo servicios de seguridad online como parte de promociones.

3. Enfoque en Clientes Nuevos: Priorizar las campañas preventivas en clientes con alta facturación y antigüedad baja (tenure), ya que son los más vulnerables.

4. Monitoreo en Tiempo Real: Implementar dashboards en Power BI que muestren a los clientes en riesgo y la pérdida potencial en tiempo real, facilitando la toma de decisiones para el equipo financiero.

## 💾 Dataset
Se utiliza un dataset simulado de clientes de una empresa de telecomunicaciones. Las variables incluidas son:

- customerID: ID único del cliente.

- gender: Género del cliente.

- SeniorCitizen: Indica si el cliente es mayor de 65 años (0=No, 1=Sí).

- tenure: Meses de permanencia como cliente.

- InternetService: Tipo de servicio de internet.

- Contract: Tipo de contrato (mensual, anual, bianual).

- MonthlyCharges: Cargo mensual en USD.

- TotalCharges: Cargo total acumulado.

- Churn: Variable objetivo (Yes/No).

(Para ver la lista completa de columnas, por favor, consulta el notebook Churn_Cost_Analysis.ipynb.)

## 🛠️ Metodología
El proyecto fue desarrollado en un entorno de Jupyter Notebook, siguiendo un flujo de trabajo estándar en Data Science:

1. Carga y Limpieza de Datos: Se procesan los datos para manejar valores nulos y asegurar la calidad del dataset.

2. Ingeniería de Características: Creación de nuevas variables como perdida_estim para estimar el costo de la pérdida de cada cliente.

3. Análisis Exploratorio (EDA): Se analizan las variables, se identifican patrones de comportamiento y se visualizan las relaciones con la variable Churn.

4. Modelado Predictivo: Se entrena un modelo de Machine Learning (XGBoost) para predecir la probabilidad de churn.

5. Evaluación y Análisis de Costos: Se evalúa el rendimiento del modelo y se calculan las pérdidas financieras potenciales para la empresa.

## 🚀 Tecnologías Utilizadas
- Lenguaje: Python

- Análisis de Datos: Pandas, Numpy

- Visualización: Matplotlib, Seaborn

- Machine Learning: Scikit-learn, XGBoost

- Interpretabilidad: SHAP (para entender las decisiones del modelo)

## 🏃‍♂️ Cómo Empezar
Clona este repositorio:
1. git clone https://github.com/tu-usuario/nombre-del-repo.git

2. Navega al directorio del proyecto:
cd nombre-del-repo

3. Asegúrate de tener un entorno de Python con las librerías necesarias. Se recomienda usar un entorno virtual.

4. Abre el notebook Churn_Cost_Analysis.ipynb en tu IDE favorito (Jupyter, VSCode, etc.) y ejecuta las celdas.

Autor: Emanuel Gallo