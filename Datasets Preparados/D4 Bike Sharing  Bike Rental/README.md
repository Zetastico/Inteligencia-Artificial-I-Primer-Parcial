Dataset 01: Bike Sharing Demand
Descripción del Dataset
Este dataset contiene el registro histórico del sistema de alquiler de bicicletas Capital Bikeshare de Washington, D.C., correspondiente a los años 2011 y 2012. La información combina datos de la duración del alquiler, fechas y horas, con variables contextuales como el clima y la estacionalidad. Es un dataset ideal para practicar el análisis de tendencias temporales y factores externos que afectan el comportamiento del usuario.

¿Qué se puede hacer con este dataset?
El objetivo principal es realizar Análisis Predictivo. Se puede entrenar un modelo de Regresión (como Random Forest Regressor o XGBoost) para pronosticar cuántas bicicletas se alquilarán en una hora o día específico. Esto es vital para que las empresas de transporte puedan:

Optimizar la logística de distribución de bicicletas.

Prever picos de demanda durante eventos o cambios climáticos.

Ajustar precios o promociones según la estación del año.

Descripción de Columnas Clave
Para este proyecto, nos enfocamos en las siguientes variables (después del preprocesamiento):

datetime: Marca de tiempo que permite extraer características como la hora del día, día de la semana y mes (clave para detectar estacionalidad).

season: Variable categórica que indica la estación (1: primavera, 2: verano, 3: otoño, 4: invierno).

holiday: Binaria (0 o 1) que indica si el día es feriado o no, afectando drásticamente el flujo de usuarios.

temp: Temperatura real en grados Celsius. Es uno de los predictores con mayor correlación con el uso de bicicletas.

atemp: Sensación térmica ("feels like"). Útil para captar el impacto del viento o la humedad en la decisión del usuario.

humidity: Porcentaje de humedad relativa; niveles muy altos suelen disminuir el alquiler de bicicletas.

windspeed: Velocidad del viento, factor que puede actuar como barrera para el uso recreativo del servicio.

count (Target): La variable objetivo. Representa el número total de alquileres (suma de usuarios casuales y registrados). Es lo que el modelo intenta predecir.
