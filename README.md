# Analisis-de-telecomunicaciones-ConnectaTel

📊 Análisis de Comportamiento del Cliente: ConnectaTel 2024
🎯 Objetivo del Proyecto
Como Analista de Datos para ConnectaTel, el objetivo principal de este proyecto fue evaluar el comportamiento de los clientes en Latinoamérica durante el periodo 2024. El análisis se enfocó en identificar patrones de consumo, detectar inconsistencias en los datos y segmentar a los usuarios para proponer estrategias de retención y optimización de planes comerciales.

📂 Estructura de Datos
El proyecto integra tres fuentes de datos principales:

plans.csv: Detalles de planes (precios, límites de minutos/GB y costos por excedentes).

users.csv: Perfil demográfico de los clientes (edad, ciudad, fecha de registro, churn).

usage.csv: Registro detallado de consumo real (llamadas y mensajes).

🛠️ Proceso de Análisis
1. Limpieza y Calidad de Datos (Data Cleaning)
Se identificaron y resolvieron problemas críticos de calidad:

Tratamiento de "Valores Centinela": Se detectaron edades con valor -999 (aproximadamente un 3% de la muestra), los cuales fueron corregidos para no sesgar el promedio de edad real (48 años).
Gestión de Nulos: Se identificó un 11.7% de registros sin información de ciudad, marcándolos como "Desconocida" para evitar pérdidas de datos en el análisis global.

2. Segmentación de Clientes
Utilizando técnicas de filtrado y agregación, se definieron dos ejes de segmentación:

Por Edad: Identificando a los "Adultos (30-55)" como el motor principal y a los "Adultos Mayores" como el grupo de mayor lealtad.

Por Nivel de Uso: Clasificación entre usuarios "Light", "Medio" e "Intensivo" basándose en el consumo real vs. los límites de su plan.

3. Hallazgos Clave (Insights)
Brecha de Valor: El promedio de llamadas es de solo 23 minutos mensuales, mientras que el plan más básico ofrece 100. Esto sugiere que muchos clientes están subutilizando sus planes.

Riesgo de Abandono: Los "Usuarios de Uso Intensivo" en planes básicos representan la mayor oportunidad de Up-selling, pero también el mayor riesgo de fuga si no se les ofrece un plan Premium competitivo.

💡 Recomendaciones de Negocio
Plan "Senior": Lanzamiento de un plan de bajo costo con alta prioridad en voz para adultos mayores.

Up-selling Automatizado: Campañas dirigidas a usuarios que superan el 90% de sus límites de datos.

Optimización de Registro: Implementar validaciones obligatorias en el sistema de captura para eliminar datos inconsistentes (como edades negativas).
