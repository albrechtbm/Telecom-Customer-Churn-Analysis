# Telecom Customer Churn Analysis
Este proyecto analiza el comportamiento de clientes de ConnectaTel utilizando datos de planes, usuarios y uso del servicio. Se realizaron procesos de limpieza, análisis exploratorio, detección de outliers y segmentación de clientes por edad y nivel de uso para identificar patrones y oportunidades de negocio.
Análisis de Clientes – ConnectaTel
Descripción del Proyecto

Este proyecto analiza el comportamiento de los clientes de ConnectaTel, una empresa de telecomunicaciones en Latinoamérica. El objetivo es comprender cómo utilizan los usuarios los servicios de llamadas y mensajes, identificar problemas de calidad en los datos y segmentar a los clientes según su comportamiento.

A partir del análisis se buscan patrones de uso, segmentos de clientes y oportunidades para mejorar la oferta de planes y estrategias de negocio.

Datasets Utilizados

El análisis utiliza tres datasets principales:

plans.csv

Contiene información sobre los planes disponibles.

Columnas principales:

plan_name

messages_included

gb_per_month

minutes_included

usd_monthly_pay

usd_per_gb

usd_per_message

usd_per_minute

users_latam.csv

Contiene información de los usuarios.

Columnas principales:

user_id

first_name

last_name

age

city

reg_date

plan

churn_date

usage.csv

Contiene el historial de uso de los servicios.

Columnas principales:

id

user_id

type (call o text)

date

duration

length

Etapas del Análisis

El proyecto sigue un flujo típico de análisis de datos.

1. Carga y exploración de datos

Se importaron los datasets y se revisó:

estructura de los datos

tipos de columnas

número de registros

valores nulos

2. Análisis de calidad de datos

Se identificaron problemas como:

valores faltantes

valores inválidos (sentinels)

inconsistencias en fechas

categorías incorrectas

3. Limpieza de datos

Se aplicaron diferentes procesos de limpieza:

reemplazo de valores inválidos en edad (-999)

estandarización de ciudades

corrección de fechas fuera de rango

validación de valores faltantes según tipo de uso

4. Agregación de uso por usuario

Se crearon métricas de comportamiento por usuario:

cantidad de mensajes enviados

número de llamadas realizadas

total de minutos en llamadas

Posteriormente se integraron estas métricas al dataset de usuarios para construir un perfil de usuario.

5. Análisis exploratorio de datos

Se utilizaron estadísticas descriptivas y visualizaciones para analizar:

distribución de edades

número de mensajes

frecuencia de llamadas

duración total de llamadas

6. Detección de Outliers

Se utilizaron:

Boxplots

Método IQR

para identificar valores extremos en:

edad

cantidad de mensajes

número de llamadas

minutos de llamadas

7. Segmentación de Clientes

Se crearon dos tipos de segmentación.

Segmentación por uso

Usuarios clasificados en:

Bajo uso

Uso medio

Alto uso

según la cantidad de llamadas y mensajes.

Segmentación por edad

Usuarios clasificados en:

Joven

Adulto

Adulto Mayor

según su rango de edad.

Principales Insights

Del análisis se identificaron algunos patrones importantes:

La mayoría de los usuarios pertenece al segmento de uso medio.

Los usuarios del plan Premium tienden a mostrar mayor actividad.

Existen usuarios con uso intensivo del servicio, que representan clientes potencialmente más valiosos.

El grupo de edad predominante corresponde a usuarios adultos.

Recomendaciones de Negocio

A partir de los hallazgos se sugieren algunas estrategias:

Crear planes especiales para usuarios de alto consumo.

Diseñar planes económicos para usuarios de bajo uso.

Implementar recomendaciones de plan basadas en el comportamiento del cliente.

Monitorear usuarios intensivos para oportunidades de up-selling.

Cómo Ejecutar el Proyecto

Este análisis puede ejecutarse en Google Colab o en un entorno de Python.

Pasos

Abrir el notebook:

ConnectaTel_analysis.ipynb

Subir los datasets al entorno de trabajo.

Ejecutar las celdas del notebook en orden.

Herramientas Utilizadas

Este proyecto fue desarrollado utilizando:

Python

Pandas

Seaborn

Matplotlib

Google Colab

GitHub

✅ Si quieres, también puedo ayudarte a agregar 3 cosas que hacen que tu repositorio se vea MUCHO más profesional:

1️⃣ Cómo agregar imágenes de tus gráficas en el README
2️⃣ Cómo dejar el README al estilo portafolio de Data Analyst
3️⃣ Cómo escribir un buen commit final para el proyecto (esto también lo revisan mucho).
