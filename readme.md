# Credit Card Fraud Detection

Este proyecto tiene como objetivo desarrollar un modelo de Machine Learning para detectar fraudes en transacciones de tarjetas de crédito. El dataset utilizado contiene transacciones realizadas por titulares de tarjetas de crédito europeas en septiembre de 2013. Con un total de 284,807 transacciones, se identificaron 492 fraudes, lo que representa solo el 0.172% de todas las transacciones, lo que hace que el problema esté altamente desequilibrado.

## Objetivos del Proyecto

- Realizar un **Análisis Exploratorio de los Datos (EDA)** para entender la estructura y distribución de las características.
- Preprocesar los datos para balancear las clases y tratar la información de manera adecuada.
- Desarrollar un **modelo de clasificación** para predecir fraudes en las transacciones.
- Evaluar el modelo utilizando métricas como el **AUC-PR** (Área bajo la Curva de Precisión-Recuerdo) debido al desequilibrio de clases en el dataset.
- Explorar diferentes enfoques de machine learning para mejorar la detección de fraudes.

## Descripción del Dataset

El dataset contiene las siguientes características:

- **V1, V2, … V28**: Componentes principales obtenidos mediante un análisis PCA. No se proporciona información sobre los atributos originales debido a problemas de confidencialidad.
- **Time**: Tiempo en segundos desde la primera transacción en el dataset.
- **Amount**: Monto de la transacción. Puede ser útil para aprender modelos sensibles a costos dependiendo del tipo de fraude.
- **Class**: Variable de respuesta que indica si la transacción es fraudulenta (`1` para fraude, `0` para no fraude).

El dataset es **altamente desequilibrado**, con la clase positiva (fraude) representando solo el 0.172% de las transacciones. Debido a este desequilibrio, se recomienda medir el desempeño del modelo utilizando el **AUPRC (Área Bajo la Curva de Precisión-Recuerdo)** en lugar de la precisión de la matriz de confusión.
