Dataset 06: Credit Approval (UCI)

Descripción del Dataset Original

Este dataset concierne a solicitudes de tarjetas de crédito. Todos los nombres de los atributos y valores han sido cambiados a símbolos sin sentido por razones de confidencialidad. Representa un reto real de Machine Learning donde el analista no conoce el contexto exacto de cada variable, obligándolo a confiar puramente en técnicas estadísticas y análisis de datos para encontrar patrones de aprobación.

¿Qué se puede hacer con este dataset?

Es un caso de uso clásico para Sistemas de Score de Crédito. El objetivo es predecir si una solicitud será aprobada o rechazada.

Clasificación Automatizada: Entrenar modelos para agilizar el proceso de aprobación de créditos bancarios.

Análisis de Relevancia: Identificar cuáles de las columnas anónimas (A1-A15) tienen mayor peso estadístico en la decisión final.

Robustez ante Datos Mixtos: Practicar el manejo de datasets que contienen una mezcla equilibrada de variables continuas y categóricas con datos faltantes.

Descripción de Columnas Clave

Debido a la anonimización, las columnas se presentan bajo etiquetas genéricas, pero el preprocesamiento identificó su importancia:

target (A16): La variable objetivo. Indica si el crédito fue aprobado (+) o rechazado (-).

A2 (Edad estimada): Variable continua que, tras la limpieza de valores nulos, representa un factor demográfico clave.

A3 (Deuda): Valor numérico que indica el nivel de endeudamiento previo del solicitante.

A8 (Años de empleo): Variable continua. Indica la estabilidad laboral, crucial para el riesgo crediticio.

A9 (Prior Default): Variable categórica binaria. Indica si el cliente ha tenido impagos anteriormente (es el predictor más fuerte del dataset).

A10 (Employed): Indica si el solicitante está empleado actualmente.

A11 (Credit Score): Un valor numérico que representa la calificación crediticia interna del banco.

A15 (Income): Nivel de ingresos del solicitante; fundamental para determinar la capacidad de pago.

Nota sobre el Preprocesamiento

El mayor desafío de este dataset fue la presencia de datos faltantes (identificados con '?') en variables críticas. Se realizó una limpieza profunda sustituyendo estos caracteres por la mediana en columnas numéricas y por la moda en las categóricas. Además, se transformaron los símbolos de la variable objetivo (+ y -) a un formato binario (1 y 0) para ser procesados por algoritmos de clasificación.
