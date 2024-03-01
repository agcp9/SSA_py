
# REGRESIÓN LINIAL 🌳

Los árboles de regresión son un tipo de modelo de regresión no lineal que se utiliza en aprendizaje automático y estadísticas para predecir valores numéricos. A diferencia de los árboles de clasificación que se utilizan para problemas de clasificación, los árboles de regresión se centran en predecir una variable continua en lugar de asignar a una categoría.




![image](https://github.com/agcp9/SSA_py/assets/71346104/356ef2a5-2a99-41d6-bfeb-c0b39bfca7a2)

## ¿Cómo funciona la regresión lineal en Python?

**- División del conjunto de datos:** El árbol comienza con el conjunto de datos completo y busca la característica que mejor divide los datos en dos conjuntos, de manera que la variabilidad en la variable de respuesta (la variable que estamos tratando de predecir) se minimice.

**- Criterio de división:** Para decidir qué característica y qué umbral utilizar en la división, se emplea un criterio de impureza, comúnmente el error cuadrático medio (MSE, por sus siglas en inglés) en el contexto de regresión. La idea es minimizar la varianza dentro de cada subconjunto resultante.

**- Construcción recursiva:** Después de la primera división, el proceso se repite en cada uno de los subconjuntos resultantes. En cada nodo, se realiza una nueva división basada en la característica que maximice la reducción en el MSE.

**- Criterio de parada:** El proceso de construcción del árbol continúa hasta que se cumple un criterio de parada, que puede ser el tamaño mínimo de los nodos terminales, la profundidad máxima del árbol o la falta de una reducción significativa en la varianza.

**- Predicción:** Una vez construido el árbol, para hacer predicciones, se sigue el camino desde la raíz hasta una de las hojas correspondientes al conjunto de características de entrada. La predicción es el valor promedio de la variable de respuesta en ese conjunto de datos de entrenamiento.

##¿En que contexto usar los arboles de regresión?

- Problemas de clasificación y regresión:
  - Clasificación:Por ejemplo, en la clasificación de correos electrónicos como spam o no spam, diagnóstico médico, clasificación de imágenes, etc.

  - Regresión:Por ejemplo, predicción de precios de viviendas, demanda de productos, etc.

- Interpretación y explicabilidad: Los árboles de decisión son fáciles de entender y visualizar, lo que los hace ideales cuando se necesita explicar las decisiones del modelo a personas no técnicas.

- Identificación de características importantes: Los árboles de decisión pueden proporcionar información sobre la importancia de cada característica en la toma de decisiones. 

- Manejo de datos mixtos: Pueden manejar conjuntos de datos que contienen características tanto categóricas como numéricas sin necesidad de una pretransformación extensa.

![image](https://github.com/agcp9/SSA_py/assets/71346104/26e9e607-36b5-4bae-93a1-5fd736ddec36)


## RESUMEN 🌳

Los árboles de regresión tienen la ventaja de ser interpretables y fáciles de visualizar. Sin embargo, pueden ser propensos al sobreajuste, especialmente si no se controla su crecimiento adecuadamente mediante técnicas como la poda (pruning). Para mejorar la generalización, a menudo se utilizan técnicas como bosques aleatorios o gradient boosting, que combinan múltiples árboles de regresión.

