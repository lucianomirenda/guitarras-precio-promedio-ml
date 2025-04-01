# **Proyecto de Ingeniería de Datos: Análisis de Guitarras en Mercado Libre** 

La idea de este proyecto era crear un pipeline completo de análisis de datos, desde la **extracción** hasta la **visualización**, basándome en un tema que es de mi interés personal y también de muchas otras personas (que también son músicos): el precio de los instrumentos, específicamente en este caso, **guitarras**.

- ¿Cuáles son las más baratas?
- ¿Cuáles son las más caras?
- ¿Existe un precio intermedio?

Estas son el tipo de preguntas que intento responder con mi proyecto.  

## **1. Extracción de datos con Python** 

Utilicé **BeautifulSoup** y **Requests** para realizar un **web scraping** en Mercado Libre, extrayendo los datos de las guitarras según ciertas características. Los datos obtenidos se organizaron en un **DataFrame** con la ayuda de **Pandas** , y luego los exporté como archivos **CSV** (uno por cada marca) .

## **2. Transformación de datos con PySpark en Databricks** 

Una vez que obtuve los datos, los llevé a **Databricks** y utilicé **PySpark** para limpiarlos y procesarlos, quitando valores nulos, agregando valores nuevos y demás.

## **3. Almacenamiento en la base de datos de Databricks** 

Transformé los datos en un **esquema estrella**, creando las tablas de **dimensiones** y **hechos**, y las almacené en una base de datos dentro de Databricks 🗃. 

## **4. Análisis con SQL dentro de Databricks** 

Después, realicé diversas **consultas SQL** directamente en Databricks para analizar los datos y obtener **promedios de precios** basados en características clave como marca, modelo y tipo de guitarra . Estas consultas me permitieron responder las preguntas de las que hablaba al principio.

## **5. Visualización de datos con Power BI** 

Para presentar los resultados de manera clara y visual, importé los datos a **Power BI** y realicé varias visualizaciones que exporte como un archivo PDF. En estas podemos ver las guitarras con un precio menos a 600mil pesos (Las más baratas) y también las más caras (con un precio mayor a 2 M de pesos). 

---
