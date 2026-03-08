<h1>Challenge 2  ALURA-LATAM  Parte 2 </h1>
<h2>          
Telecom X-Parte 2  (Data Science / Machine Learning)

Elaborado por: Mario Fco. Monzón 
</h2>

---
## Introducción

<p>La empresa Telecom X enfrenta una alta tasa de cancelaciones y necesita comprender los factores que llevan a la pérdida de clientes. 

Esta evasión de clientes representa un problema relevante para el negocio, ya que impacta directamente en la estabilidad y en los ingresos. A través del análisis de datos, se busca generar información que sirva como base para futuras estrategias de retención y modelos predictivos.

El objetivo principal, utilizando Python y sus principales bibliotecas, se centra en predecir la cancelación de clientes en telecomunicaciones mediante análisis de datos y modelos de machine learning.

</p>


---

## Descripción del proyecto

Este proyecto tiene como objetivo analizar los factores asociados a la cancelación de clientes en una empresa de telecomunicaciones y desarrollar modelos de machine learning capaces de predecir qué clientes tienen mayor probabilidad de abandonar el servicio.

El análisis incluye etapas de exploración de datos, preparación, modelado predictivo e interpretación de resultados.

***



## Objetivos del proyecto

- Identificar los factores que influyen en la cancelación de clientes
- Preparar los datos para su uso en modelos de Machine Learning.
- Analizar el balance de clases y su impacto en el modelado.
- Entrenar y comparar distintos modelos de clasificación.
- Evaluar el desempeño mediante métricas apropiadas para problemas de churn.
- Interpretar la importancia de las variables más relevantes.
- Generar conclusiones y recomendaciones estratégicas basadas en los resultados.


**************************************


## Etapas del proyecto



## Preparación y preprocesamiento de datos

En esta etapa se realizaron las siguientes tareas:

- Carga del archivo tratado en la Parte 1 del proyecto.
- Eliminación de columnas irrelevantes para el modelado (identificadores).
- Codificación de variables categóricas mediante **One-Hot Encoding**.
- Separación de variables numéricas y categóricas utilizando `ColumnTransformer`.
- Análisis de la proporción de churn para detectar desbalance de clases.
- Normalización aplicada únicamente a los modelos sensibles a la escala.

---

## **Modelado Predictivo**

Se entrenaron cinco modelos:
- Baseline (DummyClassifier)
- Regresión Logística
- Árbol de Decisión
- Random Forest
- KNN

Los modelos fueron evaluados utilizando métricas estándar:
- Accuracy
- Precision
- Recall
- F1-score
- Matrices de confusión (valores absolutos y normalizados)

Se priorizaron métricas como **Recall** y **F1-score**, considerando el desbalance moderado de clases y la importancia de detectar clientes con riesgo de evasión.


---

## Resultados

El modelo de Regresión Logística balanceada presentó el mejor desempeño para este problema, destacándose especialmente en la detección de clientes en riesgo de cancelación (mayor recall).

Esto es especialmente relevante en problemas de churn, donde el objetivo principal es anticipar la cancelación y permitir acciones de retención.

---

## Importancia de las variables

A partir del modelo seleccionado (Regresión Logística), se analizó la contribución de las variables al proceso de predicción.

Los resultados indican que la evasión de clientes está principalmente asociada a:

- Baja antigüedad del cliente.
- Contratos de corto plazo.
- Determinadas configuraciones de servicios y cargos.

Por el contrario, una mayor permanencia y contratos de mayor duración actúan como factores protectores frente al churn.

---

## Conclusiones

El modelo de **Regresión Logística** presentó el mejor desempeño general, logrando un equilibrio adecuado entre precisión y capacidad de detección de clientes que cancelan.

El análisis confirma que la evasión de clientes no depende de un único factor, sino de la combinación de variables contractuales, económicas y de relación con el servicio. La utilización de modelos predictivos permite anticipar comportamientos de riesgo y orientar acciones preventivas basadas en datos.

---

## Recomendaciones estratégicas

- Implementar estrategias de retención temprana para clientes con baja antigüedad.
- Incentivar la migración hacia contratos de mayor duración.
- Priorizar acciones comerciales sobre clientes identificados como de alto riesgo.
- Integrar el modelo predictivo como sistema de alerta temprana dentro del negocio.

---


## Herramientas utilizadas

- Google Colab
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  
 
---
