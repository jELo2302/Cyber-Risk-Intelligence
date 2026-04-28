CYBER-RISK INTELLIGENCE: SCORING DE RIESGO Y DETECCIÓN PREDICTIVA
Autor: Julián Esteban León Ospina

Descripción del Proyecto
Este ecosistema analítico está diseñado para identificar, clasificar y predecir riesgos operativos en el sector 
financiero colombiano, enfocándose en la transición de delitos tradicionales hacia modalidades informáticas. 
El proyecto se divide en dos fases críticas que transforman datos crudos en una herramienta de Scoring de 
Riesgo para la toma de decisiones preventivas.

Estructura del Repositorio
1. Parte I: Inteligencia de Datos y Análisis Espacial (EDA)
Ubicación: bank_EDA.ipynb

Auditoría de Vulnerabilidades: Análisis de patrones delictivos por departamentos.

Validación Estadística: Implementación del test Chi-cuadrado para confirmar que la distribución de delitos
varía significativamente por región, rechazando la hipótesis de uniformidad.

Geospatial Insights: Identificación de Hotspots delictivos y evolución temporal de modalidades.

2. Parte II: Modelado Predictivo y Clasificación (ML)
Ubicación: bank_ML.ipynb

Algoritmo: Implementación de XGBoost Classifier para la detección de incidentes de alto impacto.

Scoring de Riesgo: Generación de un modelo de probabilidad para clasificar transacciones y comportamientos 
sospechosos.

Evaluación Robusta: Uso de Curvas ROC (AUC > 0.85) y matrices de confusión para garantizar la fiabilidad 
del modelo frente al desbalance de clases delictivas.

Feature Importance: Análisis de variables clave (ubicación, hora, modalidad) para entender qué factores disparan el riesgo crítico.

3. Parte III: Business Intelligence (Dashboard)
Ubicación: /dashboards/CyberRisk_Analytics.pbix

Monitoreo en Tiempo Real: Visualización de la concentración delictiva (Bogotá, Medellín, Cali como focos principales).

Análisis Comparativo: Evolución de delitos informáticos vs. tradicionales.

Filtros Dinámicos: Segmentación por género, día de la semana y tipo de arma/modalidad para perfiles de riesgo detallados.

Tecnologías Utilizadas
Python 3.x: (Pandas, Numpy, Scikit-Learn, Statsmodels, Geopandas).

Machine Learning: XGBoost (Clasificación Masiva).

Estadística: Pruebas de hipótesis (Chi-square).

Visualización: Power BI (Frontend Ejecutivo) & Seaborn/Matplotlib (Frontend Técnico).

Hallazgos Estratégicos
Heterogeneidad Regional: El riesgo no es uniforme; departamentos como Cundinamarca y Antioquia presentan 
vectores de ataque distintos, lo que exige protocolos de seguridad diferenciados.

Poder de la Modalidad: La variable "Familia de Delito" es el predictor más fuerte. Sin embargo, el contexto temporal
(mes/día) aporta una capacidad predictiva complementaria vital para alertas tempranas.

Hacia lo Digital: El análisis confirma una migración sostenida hacia delitos informáticos, requiriendo que la banca 
tradicional evolucione sus modelos de scoring de clientes.