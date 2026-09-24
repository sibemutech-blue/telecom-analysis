# 📊 Proyecto de Análisis de Clientes – ConnectaTel

## 🎯 Objetivo
Evaluar el comportamiento de los clientes de **ConnectaTel** en Latinoamérica hasta el año 2024, con el fin de:
- Construir perfiles estadísticos de clientes.
- Detectar comportamientos atípicos (outliers).
- Crear segmentos de clientes por edad y nivel de uso.
- Proponer estrategias de retención y mejoras en los planes ofrecidos.

---

## 📂 Datasets utilizados
- **plans.csv** → Información de los planes actuales (precio, minutos, GB incluidos, costo por extra).  
- **users_latam.csv** → Información de los clientes (edad, ciudad, fecha de registro, plan, churn).  
- **usage.csv** → Detalle del uso real de los servicios (llamadas y mensajes).  

---

## 🧩 Etapas del análisis
1. **Carga y exploración de datos** → Validación de estructura y primeras observaciones.  
2. **Identificación de problemas de calidad** → Nulos, valores inválidos y sentinels.  
3. **Limpieza básica** → Corrección de sentinels, fechas imposibles y estandarización.  
4. **Resumen estadístico** → Métricas descriptivas por usuario y plan.  
5. **Visualización de distribuciones y outliers** → Histogramas y boxplots.  
6. **Segmentación de clientes** → Clasificación por edad y nivel de uso.  
7. **Insights ejecutivos** → Conclusiones y recomendaciones para ConnectaTel.  

---

## ✅ Correcciones aplicadas
- Filtro de usuarios → ahora incluye todos los registros hasta 2024 (no solo los de 2024).  
- Fechas futuras → se marcan como nulas con límite fijo (2024-12-31).  
- IQR → corregido a percentiles 25 y 75.  
- Categorías de uso → estandarizadas a `'call'` y `'text'`.  
- Conteos y placeholders → corregidos (users = 4000 filas, no 40,000).  

---

## 📊 Resultados principales
- **Usuarios válidos:** 3960 hasta 2024.  
- **Edad mediana:** 48 años.  
- **Planes:** 65% Básico, 35% Premium.  
- **Mensajes promedio:** 5.5 por usuario.  
- **Llamadas promedio:** 4.5 por usuario, con duración media de 23 minutos.  
- **Ciudades clave:** Bogotá y CDMX concentran la mayor base de clientes.  
- **Outliers:** heavy users detectados con IQR correcto, se mantienen como casos reales.

---

## 📑 Resumen ejecutivo
El análisis de ConnectaTel muestra que la mayoría de los clientes pertenecen al plan Básico (65%), con una edad mediana de 48 años. Los usuarios Premium presentan mayor intensidad de uso, enviando más mensajes y acumulando más minutos de llamadas. Bogotá y CDMX concentran la mayor proporción de clientes, lo que sugiere oportunidades de segmentación regional.  
La corrección de fechas y sentinels asegura que el análisis se limite al periodo válido (2022–2024), evitando sesgos. Los heavy users identificados son un segmento valioso para estrategias de fidelización.  
En conclusión, el estudio refleja fielmente el comportamiento de toda la base de clientes hasta 2024, permitiendo diseñar estrategias de retención y optimización de planes basadas en datos completos y consistentes.

---

## ⚙️ Cómo ejecutar el notebook
1. Abre [Google Colab](https://colab.research.google.com/).  
2. Sube el archivo del notebook (`ConnectaTel.ipynb`).  
3. Asegúrate de tener los datasets en la carpeta `/datasets/`.  
4. Ejecuta las celdas en orden para reproducir el análisis.  

---

## 📌 Guía de reproducción
- **Requisitos previos:** Python 3.9+, librerías `pandas`, `numpy`, `matplotlib`, `seaborn`.  
- **Pasos básicos:**
  ```bash
  pip install pandas numpy matplotlib seaborn
  
