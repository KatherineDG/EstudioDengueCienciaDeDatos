<h1>Descripción</h1>

Este proyecto realiza un análisis exhaustivo del reporte epidemiológico de dengue en la Ciudad Autónoma de Buenos Aires, integrando datos meteorológicos y poblacionales para identificar patrones, validar hipótesis y desarrollar modelos predictivos de Machine Learning.

<h2>Dataset Principal</h2>

- <b>Fuente:</b> <a href="https://data.buenosaires.gob.ar/dataset/reporte-epidemiologico-de-dengue" target="_blank">Reporte Epidemiológico del Dengue - Buenos Aires Data</a>
- <b>Rubro:</b> Salud
- <b>Fecha de publicación:</b> 17 de Mayo del 2023 (en actualización semanal)

<h1>Valor Aportado</h1>

El análisis permite transformar datos crudos en decisiones estratégicas para:
1. <b>Reducir casos y mortalidad</b>: Identifición de puntos críticos para intervención inmediata.
2. <b>Optimimzar recursos públicos</b>: Mejor distribución de presupuestos en fumigación y centros de salud.
3. <b>Campañas de concientización y ayuda</b>: Segmentación por grupos etarios más vulnerables.

<h3>Hipótesis Planteadas</h3>

- <b>Vulnerabilidad social:</b> Jóvenes y adultos tienen mayor riesgo debido a la movilidad por estudio, trabajo y ocio.
- <b>Vulnerabilidad Biológica:</b> Los grupos etarios de infancia y vejez son más propensos por sistemas inmunológicos en desarrollo o debilitados.
- <b>Factor Climático:</b> La temperatura, humedad y precipitaciones influyen directamente en el ciclo de reproducción del mosquito <i>Aedes aegypti</i>.

<h1>Limpieza y Transformación de Datos</h1>

Se aplicaron 5 técnicas principales para asegurar la calidad de los datos:
1. Suplantación estimativa de datos faltantes: Uso de datasets auxiliares de población para estimar valores de comuna o grupo_etario faltantes.
2. Normalización de texto.
3. Eliminación de duplicados.
4. Validación de Integridad.
5. Enriquecimiento del Dataset Principal.

<h1>Machine Learning</h1>

Modelos para predecir el impacto del dengue:
- <b>Random Forest Classifier:</b> Para clasificar la probabilidad de brotes en comunas específicas.
- <b>Regresión Lineal:</b> Para estimar la cantidad de casos confirmados por laboratorio en semanas futuras.
- <b>Regresión Logística:</b> Para predecir la probabilidad de infección.

<h1>Stack Tecnológico</h1>

- <b>Lenguaje de programación</b>: Python
- <b>Librerías</b>: Pandas, Scikit-learn, GeoPandas, NumPy
- <b>Visualización externa</b>: <a href="https://lookerstudio.google.com/reporting/20bd5209-7075-47df-8d35-70b63a6903ba" target="_blank">Dashboard en Looker Studio</a>


<h1>Conclusiones</h1>

- Un hallazgo es que los casos suben drásticamente en los primeros 5 meses del año, en las estaciones de Verano y Otoño.
- Las zonas críticas son las comunas 11, 15, 9 y 4.
- Una propuesta sería implementar un sistema de alerta temprana basado en pronósticos meteorológicos a 15 días y una App de reporte ciudadano de criaderos.

