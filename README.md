# Clasificación de ingresos anuales con PySpark MLlib

**Curso:** Procesamiento de Datos a Gran Escala  
**Autora:** Alisson Garcia Salazar  
**Universidad:** Pontificia Universidad Javeriana

## Objetivo

Predecir si una persona tiene ingresos anuales superiores a USD 50.000
a partir de los datos del censo Adult de UCI.

## Cuaderno

[Ver el cuaderno con resultados y gráficos](./GarciaSalario_1055.ipynb)

El taller se ejecutó en el entorno Jupyter del curso. Los datos se
almacenaron en Hadoop HDFS y se procesaron con PySpark.

## Modelos evaluados

- Regresión logística
- Árbol de decisión
- Random Forest
- Gradient-Boosted Trees
- SVM lineal

## Resultados principales

La SVM lineal obtuvo el mayor F1 para la clase `>50K` (0,6528).
Gradient-Boosted Trees obtuvo la mayor exactitud (85,73 %) y la mayor
ROC-AUC (0,9085). El cuaderno incluye la exploración de datos, la tabla
comparativa, las matrices de confusión y las conclusiones.

## Datos

[Adult / Census Income — UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/20/census+income)

Para volver a ejecutar el cuaderno, se debe descargar y descomprimir el dataset.
Luego colocar los archivos de `adult.data` y `adult.test` junto al cuaderno en el Jupyter del
curso, donde están configurados Spark y Hadoop HDFS.
