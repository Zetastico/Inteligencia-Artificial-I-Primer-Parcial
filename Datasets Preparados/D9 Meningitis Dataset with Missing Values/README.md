Dataset 09: Meningitis Diagnostic Dataset

Descripción del Dataset Original

Este dataset contiene registros clínicos de pacientes con sospecha de meningitis. Es un dataset "de estrés" para cualquier Data Scientist, ya que fue diseñado intencionalmente con una alta tasa de valores nulos y ruidos en las mediciones. Incluye datos demográficos, síntomas iniciales y resultados de pruebas diagnósticas, permitiendo simular un entorno hospitalario real donde no siempre se cuenta con el expediente completo del paciente.

¿Qué se puede hacer con este dataset?

Es el escenario ideal para practicar Clasificación en Condiciones de Incertidumbre:

Triaje Médico Automático: Desarrollar un modelo que ayude a priorizar la atención de pacientes basándose en la probabilidad de tener meningitis.

Evaluación de Estrategias de Imputación: Probar si es mejor eliminar filas con nulos o usar técnicas avanzadas de recuperación de datos (como KNN Imputer).

Identificación de Síntomas Críticos: Determinar qué combinación de síntomas (fiebre, dolor de cabeza, náuseas) es más predictiva para esta enfermedad.

Descripción de Columnas Clave

Tras el riguroso proceso de limpieza y manejo de nulos, estas son las 8 columnas más relevantes:

total (Target): El diagnóstico final. Indica si el paciente fue confirmado con meningitis (1) o no (0).

age: Edad del paciente. La meningitis afecta de manera muy distinta a niños, adultos y ancianos.

gender: Género del paciente, procesado para ser utilizado en modelos binarios.

fever: Variable binaria que indica la presencia de fiebre alta, uno de los síntomas cardinales.

headache: Reporte de dolor de cabeza intenso, síntoma común en la inflamación de las meninges.

nausea: Presencia de náuseas o vómitos, frecuentemente asociados a la presión intracraneal.

neck_stiffness: Rigidez de nuca, el signo clínico más específico para sospecha de meningitis.

consciousness_low: Indica si el paciente presenta niveles de conciencia disminuidos o confusión.

Nota sobre el Preprocesamiento

Este dataset representó el mayor reto técnico debido a la gran cantidad de valores faltantes. El preprocesamiento no solo implicó la limpieza de nulos mediante imputación estadística (mediana y moda), sino también la estandarización de etiquetas que venían con errores tipográficos. Se puso especial cuidado en no sesgar la variable objetivo, asegurando que los registros imputados mantuvieran la coherencia clínica necesaria para un diagnóstico médico.
