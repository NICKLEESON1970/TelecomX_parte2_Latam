# TelecomX_parte2_Latam
# Análisis de Evasión de Clientes - Telecom X (Parte 2)

## Descripción del Proyecto

Este proyecto se enfoca en el análisis de la evasión de clientes (churn) en una empresa de telecomunicaciones utilizando técnicas de Ciencia de Datos y Machine Learning. El objetivo es identificar los factores clave que influyen en la cancelación de servicios y proponer estrategias de retención basadas en los resultados obtenidos.

## Contenido del Repositorio

- **datos_tratados.csv**: Archivo CSV con los datos tratados y limpios.
- **notebook.ipynb**: Notebook de Google Colab con el análisis completo.
- **informe_analisis_churn.txt**: Informe detallado con los resultados del análisis.

## Pasos a Seguir

1. **Cargar el Notebook en Google Colab**:
   - Ve a [Google Colab](https://colab.research.google.com/ ).
   - Inicia una nueva libreta.
   - Copia y pega el contenido del archivo `notebook.ipynb` en la libreta.

2. **Ejecutar el Notebook**:
   - Ejecuta cada celda del notebook para realizar el análisis completo.
   - Asegúrate de que no haya errores en la ejecución.

3. **Revisar los Resultados**:
   - Los resultados del análisis se guardarán en el archivo `informe_analisis_churn.txt`.
   - Revisa el archivo `informe_analisis_churn.txt` para obtener una conclusión detallada y las estrategias de retención propuestas.

## Explicación Detallada de los Cambios y Mejoras

### Exploración Inicial
- Se han agregado impresiones detalladas de las primeras filas, información general, resumen estadístico y columnas del DataFrame para una revisión completa.

### Eliminación de Columnas Irrelevantes
- Se ha eliminado la columna `customerID` y se pueden agregar más columnas irrelevantes si es necesario.

### Separación de Columnas Numéricas y Categóricas
- Se han separado las columnas numéricas y categóricas para aplicar diferentes estrategias de imputación.

### Imputación de Valores Faltantes
- Se han imputado valores faltantes en las columnas numéricas con la media.
- Se han imputado valores faltantes en las columnas categóricas con la moda.

### Codificación de Variables Categóricas
- Se han codificado todas las variables categóricas en formato numérico usando `pd.get_dummies`.

### Verificación de la Proporción de Cancelación
- Se ha calculado la proporción de clientes que cancelaron para evaluar el desbalanceo de clases.

### Balanceo de Clases
- Se ha aplicado `SMOTE` para equilibrar las clases y evitar sesgos en los modelos.

### Normalización
- Se ha normalizado el conjunto de datos para mejorar el rendimiento de los modelos basados en distancia.

### Análisis de Correlación
- Se ha visualizado la matriz de correlación para identificar relaciones entre las variables numéricas.

### Análisis Dirigido
- Se han creado gráficos para analizar la relación entre el tiempo de contrato y la cancelación, así como entre el gasto total y la cancelación.

### Separación de Datos
- Se han dividido los datos en conjuntos de entrenamiento y prueba con una proporción de 80/20.

### Creación de Modelos
- Se han creado tres modelos: Regresión Logística, Random Forest y Support Vector Machine (SVM).

### Evaluación de los Modelos
- Se han evaluado los modelos utilizando métricas como exactitud, precisión, recall, F1-score y matriz de confusión.
- Se han visualizado las matrices de confusión para cada modelo.

### Análisis de la Importancia de las Variables
- **Regresión Logística**: Se han analizado los coeficientes de las variables.
- **Random Forest**: Se ha utilizado la importancia de las variables proporcionadas por el modelo.
- **Support Vector Machine (SVM)**: No proporciona importancia de características directamente, pero se han utilizado los resultados de Random Forest para inferir las variables más importantes.

### Conclusión
- Se ha elaborado un informe con los factores principales que afectan la cancelación y se han propuesto estrategias de retención basadas en estos factores.

### Guardado del Informe
- Se ha guardado el informe completo en un archivo de texto llamado `informe_analisis_churn.txt` para su revisión y entrega.

## Ejecución en Google Colab

1. **Abrir Google Colab**:
   - Ve a [Google Colab](https://colab.research.google.com/ ).
   - Inicia una nueva libreta.

2. **Copiar y Pegar el Script**:
   - Copia el script completo proporcionado en el archivo `notebook.ipynb` y pégalo en una celda de la libreta.

3. **Ejecutar la Celda**:
   - Ejecuta la celda para cargar los datos y realizar el análisis completo.

Este script debería ejecutarse sin errores y proporcionar los resultados esperados, incluyendo las métricas de evaluación de los modelos y las estrategias de retención basadas en los factores más importantes identificados.

## Informe Final

El informe final se guardará en un archivo de texto llamado `informe_analisis_churn.txt` y contendrá:

- **Exploración Inicial**: Información sobre las primeras filas, información general, resumen estadístico y columnas del DataFrame.
- **Eliminación de Columnas Irrelevantes**: Se eliminarán columnas como `customerID`.
- **Manejo de Valores Nulos**: Se imputarán valores faltantes en las columnas numéricas con la media y en las columnas categóricas con la moda.
- **Codificación de Variables Categóricas**: Todas las variables categóricas serán codificadas en formato numérico usando `pd.get_dummies`.
- **Verificación de la Proporción de Cancelación**: Se calculará la proporción de clientes que cancelaron.
- **Balanceo de Clases**: Se aplicará `SMOTE` para equilibrar las clases.
- **Normalización**: Se normalizará el conjunto de datos.
- **Análisis de Correlación**: Se visualizará la matriz de correlación.
- **Análisis Dirigido**: Se crearán gráficos para analizar la relación entre el tiempo de contrato y la cancelación, así como entre el gasto total y la cancelación.
- **Separación de Datos**: Se dividirán los datos en conjuntos de entrenamiento y prueba.
- **Creación de Modelos**: Se crearán tres modelos: Regresión Logística, Random Forest y Support Vector Machine (SVM).
- **Evaluación de los Modelos**: Se evaluarán los modelos utilizando métricas como exactitud, precisión, recall, F1-score y matriz de confusión.
- **Análisis de la Importancia de las Variables**: Se analizarán los coeficientes de la Reg
