Dataset 02: MIMIC-III Clinical Database (Demo)

Descripción del Dataset Original

MIMIC-III es una base de datos de acceso abierto que contiene datos de salud anonimizados de pacientes que ingresaron en unidades de cuidados intensivos (UCI). El dataset es de naturaleza relacional, compuesto por múltiples tablas vinculadas por identificadores únicos (subject_id, hadm_id). Para este proyecto, se utilizó la versión Demo, que incluye registros completos de 100 pacientes para permitir el desarrollo de algoritmos sin comprometer la privacidad de datos a gran escala.

¿Qué se puede hacer con este dataset?

Es uno de los datasets más potentes para la IA en Salud. Con el procesamiento realizado, el dataset está listo para:

Predicción de Mortalidad Hospitalaria: Entrenar modelos de clasificación para identificar pacientes con alto riesgo de fallecimiento.

Estimación de Estancia (LOS): Predecir cuántos días permanecerá un paciente en la UCI.

Análisis de Comorbilidades: Estudiar cómo la cantidad y tipo de diagnósticos (ICD-9) afectan los resultados clínicos.

Monitoreo de Estabilidad: Analizar la fluctuación de los resultados de laboratorio durante el ingreso.

 Descripción de Columnas Clave (Consolidadas)
Tras realizar un proceso de agregación y limpieza, estas son las columnas más importantes del dataset final:

hospital_expire_flag (Target): Indica si el paciente falleció durante su estancia en el hospital (1) o fue dado de alta (0).

age_at_admit: Edad del paciente al momento del ingreso. Nota: Los valores >89 años fueron normalizados a 90 según el protocolo de anonimización de MIMIC.

lab_count: Cantidad total de exámenes de laboratorio realizados durante el ingreso. Es un indicador de la complejidad del caso.

lab_mean: El promedio de todos los valores numéricos de laboratorio. Representa un estado clínico general.

lab_max / lab_min: Valores extremos alcanzados en pruebas críticas, esenciales para detectar crisis de salud.

total_diseases: Conteo de diagnósticos registrados para el ingreso (extraído de la tabla DIAGNOSES_ICD).

gender_M: Variable binaria (One-Hot Encoding) para el género del paciente.

admission_type: Clasificación del ingreso (Emergency, Urgent, Elective), crucial para entender la urgencia médica.
