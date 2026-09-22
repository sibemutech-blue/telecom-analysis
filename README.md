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
