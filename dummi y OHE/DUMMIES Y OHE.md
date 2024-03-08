# "dummy variables" (variables ficticias) Y "One-Hot Encoding" (OHE)

Las "dummy variables" (variables ficticias) y la codificación "One-Hot Encoding" (OHE) son técnicas utilizadas en análisis de datos y modelado estadístico para manejar variables categóricas. Ambas técnicas transforman las variables categóricas en una forma numérica que los modelos de machine learning pueden entender y procesar más fácilmente. Aunque son conceptos similares, a menudo se aplican en contextos ligeramente diferentes.

## Dummy Variables:

Las variables ficticias son una forma de convertir variables categóricas en variables numéricas. Cuando una variable categórica tiene n categorías, se crean n-1 variables ficticias. Esto se hace para evitar la multicolinealidad en modelos lineales, ya que la inclusión de todas las n variables ficticias llevaría a que una sea una combinación lineal de las otras, lo cual puede afectar la estabilidad del modelo. Por ejemplo, si una variable categórica tiene tres categorías (A, B, C), se crean dos variables ficticias: una que tiene un valor de 1 cuando la categoría es A (y 0 de lo contrario) y otra para B (también 0 o 1). La categoría C se representa cuando ambas variables ficticias son 0.

## One-Hot Encoding (OHE):

One-Hot Encoding es una técnica específica de codificación de variables categóricas que convierte cada categoría en una nueva variable binaria (0 o 1). A diferencia de las variables ficticias, en OHE se crea una variable binaria para cada categoría. Si una variable categórica tiene n categorías, se crean n variables en la codificación one-hot. Cada una de estas variables binarias representa la presencia (1) o ausencia (0) de una categoría. OHE es muy utilizado en machine learning, especialmente cuando no hay un orden inherente en las categorías y cuando el modelo no asume linealidad.

# Diferencias clave:

- La principal diferencia radica en el número de variables creadas: n-1 para dummy variables en el contexto de modelos lineales para evitar la multicolinealidad, y n para one-hot encoding, que es ampliamente usado en contextos donde la multicolinealidad no es una preocupación, como en modelos de árboles de decisión o redes neuronales.

- La elección entre usar dummy variables o one-hot encoding puede depender del tipo de modelo que se está utilizando y del contexto específico del análisis.
