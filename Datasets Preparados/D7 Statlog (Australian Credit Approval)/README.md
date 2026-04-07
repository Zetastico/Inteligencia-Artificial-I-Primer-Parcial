Dataset 07: Australian Credit Approval (Statlog)

Descripción del Dataset Original

Este dataset proviene del proyecto Statlog y se centra en solicitudes de crédito en Australia. Al igual que otros datasets financieros de la época, todos los nombres de los atributos y valores han sido anonimizados (A1 a A14) para proteger la privacidad de los clientes y las políticas internas del banco. Es un dataset muy valorado para probar la robustez de algoritmos de clasificación en escenarios de "caja negra" (donde no conocemos el significado real de las variables).

¿Qué se puede hacer con este dataset?

Es ideal para el desarrollo de Modelos de Clasificación Robusta. Al tener una distribución de clases casi perfecta (45% positivos, 55% negativos), permite:

Benchmarking de Algoritmos: Comparar la precisión de modelos como SVM, Random Forest y Redes Neuronales sin preocuparse por el desbalance de clases.

Reducción de Dimensionalidad: Aplicar técnicas como PCA (Análisis de Componentes Principales) para ver si las 14 variables anónimas pueden simplificarse.

Evaluación de Generalización: Verificar si un modelo entrenado aquí puede adaptarse a otros datasets de crédito.

Descripción de Columnas Clave

Aunque las columnas son anónimas, el preprocesamiento identificó la naturaleza de los datos para su correcta codificación:


target (A15): La variable objetivo. 1 para solicitud aprobada, 0 para rechazada.

A1 (Categórica): Generalmente asociada al género o estado civil del solicitante.

A2 (Continua): Representa un valor numérico de magnitud media (frecuentemente asociado a la edad).

A4 / A5 / A6: Variables categóricas que representan el perfil socio-profesional.

A7 (Continua): Un indicador de historial o comportamiento financiero previo.

A8 (Booleana): Indica una condición específica (probablemente historial de impagos).

A10 (Numérica): Conteo de algún factor de riesgo o puntos de score.

A14 (Continua): Nivel de ingresos o capital disponible.

Nota sobre el Preprocesamiento

Este dataset es notablemente más limpio que el Credit Approval (UCI), sin embargo, el reto principal fue asegurar que las variables continuas no tuvieran sesgo por valores atípicos (outliers). Se aplicó un escalado estándar y se verificó la integridad de las categorías. Al ser un dataset balanceado, se conservó la estructura original para permitir que el modelo aprenda de una muestra representativa de éxitos y fracasos crediticios.
