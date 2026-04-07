Dataset 08: Breast Cancer Wisconsin (Original)

Descripción del Dataset Original

Este dataset fue creado por el Dr. William H. Wolberg de la Universidad de Wisconsin. A diferencia de otros datasets médicos que usan sensores automáticos, este se basa en el examen microscópico de muestras de tejido obtenidas mediante Aspiración con Aguja Fina (FNA). Los patólogos evaluaron diferentes características de los núcleos celulares en una escala del 1 al 10, donde 1 es lo más cercano a la normalidad y 10 es lo más cercano a una patología severa.

¿Qué se puede hacer con este dataset

Es el escenario perfecto para trabajar en Diagnóstico Asistido por Computadora (CAD). El objetivo principal es la Clasificación Binaria:

Detección de Malignidad: Clasificar automáticamente si un tumor es Benigno o Maligno.

Reducción de Biopsias Innecesarias: Ayudar a los médicos a identificar con alta precisión casos benignos que no requieren procedimientos invasivos adicionales.

Análisis de Correlación Celular: Entender qué características del núcleo (como la mitosis o la cromatina) son los indicadores más fuertes de cáncer.

Descripción de Columnas Clave:

class (Target): La variable objetivo. Representa el diagnóstico final (2 para Benigno, 4 para Maligno). Nota: En el preprocesamiento se transformó a 0 y 1.

Clump Thickness: Evalúa si las células están agrupadas en capas simples o en múltiples capas.

Uniformity of Cell Size: Mide la consistencia en el tamaño de las células; la disparidad suele ser señal de cáncer.

Uniformity of Cell Shape: Evalúa si la forma de las células es constante o irregular.

Marginal Adhesion: Las células normales tienden a pegarse entre sí; las cancerosas pierden esta capacidad.

Single Epithelial Cell Size: El agrandamiento de la célula epitelial es un indicador clínico importante.

Bare Nuclei: Se refiere a los núcleos que no están rodeados de citoplasma. Esta columna suele tener datos faltantes que fueron imputados.

Bland Chromatin: Describe la textura del núcleo; en las células cancerosas, la cromatina suele ser más gruesa.

Nota sobre el Preprocesamiento

El desafío principal de este dataset fue la columna Bare Nuclei, la cual contenía valores nulos (marcados originalmente como '?'). Se aplicó una imputación por la moda dado que la distribución de los datos es discreta (1-10). Además, se realizó un mapeo de la variable objetivo de su formato original (2 y 4) a un formato binario estándar (0 y 1) para facilitar el entrenamiento de modelos de red neuronal y regresión logística.
