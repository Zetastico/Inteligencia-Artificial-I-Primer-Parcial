Dataset 05: Adult Income (Census Income)

Descripción del Dataset Original

Este dataset fue extraído de la base de datos del censo de Estados Unidos de 1994 por Ronny Kohavi y Barry Becker. Contiene información demográfica y laboral de miles de individuos. Es un dataset de referencia para probar algoritmos de clasificación, ya que presenta desafíos reales como datos faltantes (etiquetados con "?") y una distribución de clases desequilibrada.

¿Qué se puede hacer con este dataset?

Es el escenario perfecto para trabajar en Modelos de Clasificación Binaria. El objetivo es predecir si una persona gana más o menos de $50,000 anuales basándose en su perfil demográfico.

Predicción Socioeconómica: Identificar los factores que más influyen en el nivel de ingresos.

Detección de Sesgos (Fairness): Analizar si el modelo presenta sesgos injustos por género o etnia (un tema muy avanzado en ética de IA).

Segmentación de Mercado: Entender el poder adquisitivo de diferentes grupos poblacionales para campañas dirigidas.

Descripción de Columnas Clave:

income (Target): La variable objetivo binaria. Indica si el ingreso es >50K o <=50K.

age: Edad de la persona. Suele haber una correlación positiva entre la edad/experiencia y el nivel de ingresos.

workclass: Tipo de empleo (Privado, Gobierno, Independiente, etc.). Define la estabilidad y el rango salarial.

education-num: Nivel educativo expresado de forma numérica (años de estudio). Es mucho más útil para el modelo que la descripción textual del título.

marital-status: Estado civil. Estadísticamente, en este dataset, es un fuerte predictor del nivel de ingresos.

occupation: El campo laboral específico. Diferencia niveles de ingresos entre áreas técnicas, administrativas o de servicios.

hours-per-week: Cantidad de horas trabajadas a la semana. Crucial para distinguir entre empleos de tiempo completo y parcial.

capital-gain / capital-loss: Ganancias y pérdidas de capital. Son variables de alta varianza que indican inversiones exitosas o fallidas.

Nota sobre el Preprocesamiento

En este dataset, el manejo de datos faltantes fue clave, ya que muchos registros contenían el carácter ?. Se aplicó una imputación por la moda en las variables categóricas para no perder filas valiosas. Además, debido a la gran cantidad de categorías en native-country, se realizó una agrupación para reducir la dimensionalidad antes de aplicar One-Hot Encoding.
