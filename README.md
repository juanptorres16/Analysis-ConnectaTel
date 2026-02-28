**Análisis de Uso y Segmentación de Clientes – ConnectaTel**

**Descripción del Proyecto**

Este proyecto analiza el comportamiento de uso de los clientes de ConnectaTel, una empresa de telecomunicaciones con operaciones en Latinoamérica.

El objetivo es entender cómo los clientes utilizan los servicios móviles (llamadas y mensajes), identificar patrones de consumo, detectar valores atípicos y construir segmentaciones útiles para la toma de decisiones comerciales.

El análisis incluye:
	•	Limpieza y validación de datos
	•	Agregación del uso por usuario
	•	Segmentación por nivel de uso
	•	Segmentación por edad
	•	Identificación de outliers mediante método IQR
	•	Generación de conclusiones ejecutivas para el negocio

⸻

**Datasets Utilizados**

Se trabajó con tres fuentes principales de información:
	•	plans.csv: Información de planes (precio, minutos incluidos, GB y costos adicionales).
	•	users_latam.csv: Datos de clientes (edad, ciudad, fecha de registro y plan contratado).
	•	usage.csv: Registros históricos de uso (duración de llamadas y mensajes).

⸻

**Limpieza y Preparación de Datos**

Durante la exploración se detectaron los siguientes problemas:
	•	Valores sentinela en la columna age (-999).
	•	Fechas futuras en reg_date.
	•	Valores inconsistentes en la columna city (”?”).
	•	Valores nulos estructurales en duration y length según el tipo de registro (llamada o mensaje).

Tras la limpieza y estandarización, los datos quedaron consistentes y listos para análisis.

⸻

**Segmentación de Clientes**

Segmentación por Nivel de Uso

Los usuarios fueron clasificados en tres grupos:
	•	Bajo uso
	•	Uso medio
	•	Alto uso

Resultados principales:
	•	Aproximadamente 74% de los usuarios presentan uso medio.
	•	19% corresponden a bajo uso.
	•	7% pertenecen al segmento de alto uso.

El segmento de alto uso es reducido pero estratégico, ya que concentra mayor intensidad de consumo.

⸻

**Segmentación por Edad**

Los usuarios se clasificaron en:
	•	Joven (menor a 30 años)
	•	Adulto (30 a 59 años)
	•	Adulto Mayor (60 años o más)

Distribución:
	•	50% Adultos
	•	31% Adulto Mayor
	•	19% Jóvenes

No se observaron diferencias significativas en el nivel de uso entre los distintos grupos etarios.

⸻

**Análisis de Outliers**

Se identificaron valores extremos mediante el método IQR en:
	•	Cantidad de mensajes
	•	Cantidad de llamadas
	•	Total de minutos de llamada

Los valores atípicos fueron conservados, ya que representan comportamientos reales de usuarios intensivos y potencialmente de alto valor para la empresa.

⸻

**Principales Hallazgos**
	•	La intensidad de uso es un factor de segmentación más relevante que la edad.
	•	La mayoría de los clientes presenta un consumo moderado.
	•	Existe una oportunidad clara de monetización en el segmento de alto uso.
	•	La base de clientes está compuesta principalmente por adultos en edad productiva.

⸻

**Recomendaciones Estratégicas**
	•	Diseñar estrategias de upgrade para usuarios de uso medio.
	•	Crear beneficios diferenciados para fidelizar clientes de alto uso.
	•	Optimizar la estructura de planes según patrones reales de consumo.
	•	Implementar campañas de activación para reducir el bajo uso.

⸻

**Cómo Ejecutar el Proyecto**

El notebook puede abrirse y ejecutarse en:
	•	Google Colab
	•	Jupyter Notebook
	•	VS Code

El análisis es completamente reproducible siguiendo las celdas del notebook.

⸻

**Herramientas Utilizadas**
	•	Python
	•	Pandas
	•	NumPy
	•	Seaborn
	•	Matplotlib


**Autor**

Juan Pablo Torres
Proyecto de Portafolio – Data Analytics
