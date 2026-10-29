# TFM - Predicción de Incendios Forestales

Proyecto de Trabajo Fin de Máster centrado en la predicción del riesgo de incendios forestales mediante técnicas de Machine Learning y visualización de resultados en Power BI.

## Tecnologías
- Python
- Pandas
- Scikit-learn
- Power BI
- DAX
- Power Query

## Contenido
- Dataset de municipios
- Modelo predictivo
- Resultados del Random Forest
- Modelo semántico en Power BI
- Dashboard de análisis de riesgo
- Dashboard de rendimiento del modelo

## Power BI Dashboard

An interactive Power BI dashboard was developed to explore wildfire risk, predictions and key indicators.

The report includes:

- Geographic visualization of wildfire risk
- Predicted risk analysis
- Temporal analysis
- Key KPIs and indicators
- Interactive filtering
- Semantic model developed in Power BI

## Project format

The Power BI project is stored using the PBIP format to improve version control and allow changes to the report and semantic model to be tracked in GitHub.

## Dashboard Power BI

Se ha desarrollado un dashboard interactivo en Power BI para analizar el riesgo de incendios forestales en Andalucía a nivel municipal y provincial.

### Tratamiento y preparación de los datos

Antes de construir las visualizaciones se realizó un proceso de preparación y validación de los datos:

- Normalización y revisión de los municipios para relacionar correctamente las diferentes tablas del modelo.
- Creación de una dimensión de municipios para centralizar la información geográfica.
- Revisión y corrección de las coordenadas geográficas utilizadas en el mapa.
- Corrección de variables meteorológicas que estaban siendo interpretadas incorrectamente por Power BI debido al separador decimal.
- Conversión de temperatura, humedad, precipitación y velocidad del viento a valores decimales utilizando la configuración regional adecuada en Power Query.
- Integración de las predicciones del modelo de Machine Learning con los datos territoriales.
- Creación de una tabla calendario para facilitar el análisis temporal.
- Organización del modelo semántico y sus relaciones para facilitar el análisis en Power BI.

### Visualizaciones

El dashboard incluye:

- Mapa de riesgo de incendio forestal por municipio.
- Distribución de municipios según nivel de riesgo.
- Probabilidad media de riesgo alto por provincia.
- KPIs de municipios analizados, municipios clasificados con riesgo alto y probabilidad media de riesgo.
- Indicadores meteorológicos utilizados en el análisis.
- Segmentadores para facilitar la exploración de los resultados.

### Vista del dashboard

![Dashboard de análisis de incendios forestales](images/dashboard-tfm.png)