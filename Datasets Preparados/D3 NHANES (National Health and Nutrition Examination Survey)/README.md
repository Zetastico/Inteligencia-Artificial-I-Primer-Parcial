Dataset 03: NHANES Health and Nutrition Survey

Descripción del Dataset Original

El dataset proviene de los Centros para el Control y la Prevención de Enfermedades (CDC) de los Estados Unidos. NHANES es un programa de encuestas diseñado para evaluar el estado de salud y nutrición de adultos y niños. Lo que hace único a este dataset es que combina entrevistas personales con exámenes físicos y pruebas de laboratorio (sangre, orina, etc.), proporcionando una visión integral del bienestar físico.

¿Qué se puede hacer con este dataset?

Es el estándar de oro para la Epidemiología Predictiva. Con este dataset se pueden desarrollar modelos para:

Detección Temprana de Enfermedades: Predecir condiciones como hipertensión o diabetes antes de que presenten síntomas graves.

Análisis de Factores de Riesgo: Identificar cómo el estilo de vida (dieta, actividad física) influye en biomarcadores específicos.

Modelos de Clasificación de Salud: Categorizar el estado general de un individuo basándose en métricas corporales y resultados de laboratorio.


Descripción de Columnas Clave

He procesado este dataset enfocándome en las métricas fisiológicas más determinantes:

BMXWT (Body Weight): Peso corporal del participante. Es una métrica base para calcular riesgos metabólicos.

BMXHT (Standing Height): Altura del participante, esencial para calcular el IMC (Índice de Masa Corporal).

BMXBMI (Body Mass Index): Variable calculada que sirve como un indicador primario de obesidad o desnutrición.

BPXSY1 / BPXDI1 (Blood Pressure): Lecturas de presión arterial sistólica y diastólica. Son predictores críticos para enfermedades cardiovasculares.

LBXGLU (Fastin Glucose): Niveles de glucosa en ayunas, la variable principal para identificar pre-diabetes y diabetes.

LBXTR (Triglycerides): Niveles de triglicéridos en sangre, fundamentales para evaluar el perfil lipídico.

RIAGENDR (Gender): Género del participante (clave para entender diferencias fisiológicas en los modelos).

RIDAGEYR (Age): Edad cronológica. Permite ajustar el modelo ya que muchos indicadores de salud varían naturalmente con el tiempo.
