Dataset 01: Housing Price Prediction

Descripción del Dataset Original

Este dataset contiene información detallada sobre el mercado inmobiliario, incluyendo características físicas de las propiedades y su entorno. Es un recurso clásico para el estudio de la economía urbana y el desarrollo de modelos predictivos de precios. Los datos incluyen variables tanto cuantitativas (áreas, números de habitaciones) como cualitativas (terminaciones, presencia de servicios).


¿Qué se puede hacer con este dataset?

El objetivo principal es construir un modelo de Regresión para predecir el precio de mercado de una vivienda. Con este dataset se pueden realizar las siguientes tareas:

Estimación de Valor: Crear herramientas de tasación automática para inmobiliarias.

Análisis de Sensibilidad: Determinar qué factores (como el área del terreno o el número de baños) influyen más en el costo final de una casa.

Optimización de Inversiones: Identificar propiedades que podrían estar subvaloradas según sus características técnicas.

 Descripción de Columnas Clave
He seleccionado y procesado estas 8 columnas fundamentales para el rendimiento del modelo:

price (Target): El precio de venta de la casa. Es la variable dependiente que nuestro modelo de IA intentará predecir.

area: La superficie total del terreno en pies cuadrados. Es, por lo general, el predictor con mayor correlación positiva con el precio.

bedrooms: Número de habitaciones. Indica la capacidad de la vivienda y su idoneidad para diferentes tamaños de familia.

bathrooms: Número de baños. En el mercado moderno, esta variable suele tener un peso significativo en el lujo y precio final.

stories: El número de pisos de la construcción. Afecta la distribución del espacio y la valoración arquitectónica.

mainroad: Variable binaria que indica si la casa tiene acceso a una vía principal (afecta la plusvalía y el ruido).

guestroom: Indica la presencia de una habitación adicional para invitados, un factor de valor agregado en viviendas de gama media-alta.

parking: Número de plazas de estacionamiento disponibles. Un factor crítico en zonas urbanas densas.
