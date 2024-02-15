# REGRESIÓN LOGISTICA 📈
La regresión logística es un modelo utilizado para la clasificación de datos binarios, es decir, cuando la variable dependiente es categórica y tiene dos categorías posibles. Aunque el nombre contiene la palabra "regresión", la regresión logística se utiliza comúnmente para problemas de clasificación en lugar de regresión.

## ¿Cómo funciona la regresión logistica en Python?
### 1. Función Sigmoide:
- La regresión logística utiliza la función sigmoide para transformar la salida del modelo en un valor entre 0 y 1. La función sigmoide es �(�)=11+�−�σ(z)= 1+e −z1​ , donde � z es la combinación lineal de las características.

### 2. Modelo Logístico:
- El modelo logístico es ln(�1−�)=�0+�1�1+�2�2+…+����ln( 1−pp)=β 0+β 1​x 1​+β 2x 2+…+ n n, donde �p es la probabilidad de que la variable dependiente sea igual a 1 y �0,�1,…,��β 0,β 1,…,β n son los coeficientes del modelo.

### 3. Entrenamiento:
- Los coeficientes se estiman utilizando técnicas de optimización, como el descenso de gradiente, para maximizar la verosimilitud de los datos observados.

### 4. Predicciones:
- Después de entrenar el modelo, se pueden hacer predicciones asignando una observación a la clase 1 si la probabilidad estimada es mayor a 0.5, y a la clase 0 si es menor a 0.5.

## ¿Cuándo utilizar la regresión logística✅?
La regresión logística es apropiada cuando:

- La variable dependiente es binaria (dos clases) y se busca predecir la probabilidad de pertenencia a una clase.

- Se desea entender el impacto de las variables independientes en la probabilidad de pertenencia a una clase.

Es comúnmente utilizada en problemas de clasificación binaria, como predicciones de spam/no spam, diagnósticos médicos (enfermo/sano), entre otros.

## ¿Cuándo no utilizar la regresión logística❌?
La regresión logística puede no ser apropiada cuando:

- La variable dependiente tiene más de dos categorías (en ese caso, se podrían explorar modelos de regresión logística multinomial o modelos de clasificación diferentes).

- La relación entre las variables independientes y la probabilidad no es aproximadamente lineal en el log-odds.

## RESUMEN 📈

En casos más complejos o con datos no lineales, otros modelos de clasificación, como máquinas de soporte vectorial (SVM), árboles de decisión o métodos de aprendizaje profundo, podrían ser más adecuados.