# ConectaTel-Analysis

Los datasets `users`, `plans` y `usage`  incluyen mas de 40.000 registros de servicios moviles, información de usuarios y planes móviles, los cuales contienen valores faltantes, sentinels, outliers y problemas de calidad diseñados para simular datos reales de la empresa.

## 📂 Contenido del repositorio

- `S7 Version-Estudiante-Project-ConnectaTel_VF.ipynb`
  → Notebook principal con limpieza, EDA, distribuciones, outliers y conclusiones.

## ▶ Cómo abrir el notebook en Google Colab

Haz clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eiQcGNNIXGwAsCvasjMGrtJwpm_pWcSu?usp=sharing)

O:

1. Abre el archivo `.ipynb` en GitHub
2. Haz clic en **Open in Colab**

## 📘 Cómo reproducir el análisis

1. Abre `S7 Version-Estudiante-Project-ConnectaTel_VF.ipynb`
2. Ejecuta las celdas en orden
3. El notebook carga automáticamente el dataset desde `/data/` o desde un enlace público (según corresponda)


## Resumen

En este proyecto identifiqué patrones de uso, detecté comportamientos atípicos y comprendí qué segmentos de clientes muestran necesidades diferenciadas, con el fin de optimizar la oferta comercial y mejorar la experiencia del usuario. Mediante python y pandas, realicé el cruce de fuentes entre planes, clientes y uso de los servicios. A continuación, revisamos cifras estadísticas entre planes y detectamos outliers para evitar sesgos en el análisis. Finalmente construí segmentaciones por cliente para analizar los usos de servicios de acuerdo con cada grupo.

## 🧠 Objetivo del análisis

Identificar patrones de uso, detectar comportamientos atípicos y comprender qué segmentos de clientes muestran necesidades diferenciadas, con el fin de optimizar la oferta comercial y mejorar la experiencia del usuario.


## Metodología:
-	Procesamiento de datos: se limpiaron y estandarizaron los datos, transformando tipos de datos a formato fecha, imputación de sentinels y valores imposibles.
-	Clasificación de missing data: Se determinó en que grupo de datos faltantes encajaron las columnas con esta novedad para determinar su tratamiento.
-	Unión de tablas: Se unieron las tablas usuarios y uso de servicios tabla para proceder con la visualización y análisis de los datos obtenidos.
- Agrupación de uso por usuario: Se agruparon los valores de uso por usuario según el tipo de medida del servicio para dar una vista estadística por usuario.
- Segmentaciones: Se analizaron las segmentaciones por tipo de plan y se construyó una adicional determinando el tipo de cliente.

## Herramientas y tipo de proyecto
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3776AB?style=for-the-badge&logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=seaborn&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)

- Limpieza y transformación de datos, unión de DataFrames, Distribuciones


## Visualizaciones destacadas
1.	Diagrama de plan por edad de usuario: Observamos una visualización de cantidad de usuarios por edad e incluimos una segmentación por tipo de plan. Existe una distribución organizada de acuerdo con los rangos de edad y descartamos outliers aquí.  

<img width="572" height="455" alt="image" src="https://github.com/user-attachments/assets/71c13bb9-d889-42a6-8e16-1ec693426688" />

----------------------------------------------------------------------------------------------------------------------------------------

2.	Gráfico de distribución por tipo de usuario: De acuerdo con el resultado, los usuarios adultos (entre 30 y 59 años) concentran la mayor cantidad de uso de servicios seguido de los adultos mayores (mayores de 60 años) y finalmente de los jovenes (menos de 30 años). El rango de diferencia es casi asimétrico entre cada escala.

<img width="580" height="455" alt="image" src="https://github.com/user-attachments/assets/e876caab-6ec6-4b59-b407-de2c96da014e" />


## Conclusiones y recomendaciones

- Segmentación por tipo plan: Una cantidad pequeña de usuarios, pueden estar haciendo más uso de los servicios en mayores proporciones que los demás, sin embargo, los gráficos evidencian que en los valores predomina el plan básico.

- Segmentación por edad de cliente: Se analizó que los usuarios que más utilizan los servicios se encuentran en un rango de edad entre los 30 y 59 años los cuales representan un 50% del total de usuarios.

Acciones recomendadas: 

- Revisar y mejorar las funcionalidades del plan premium.
- Realizar campañas de promociones a clientes en el rango de edad entre los 30 y 59 años, por ejemplo reduciendo el costo del plan premium, o reduciendo el costo de textos o minutos progresivamente a su duración o tamaño.
