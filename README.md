## Limpieza de Datos de Productos de Audible
### Descripción
Este proyecto está dedicado a la limpieza de datos de productos de Audible, una plataforma de audiolibros y contenido de audio. El conjunto de datos incluye columnas como author, narrator, time, releasedate, language, stars, price, y ratings. El objetivo es preparar estos datos para análisis posteriores, limpiando valores faltantes, corrigiendo formatos incorrectos y asegurando que los datos sean coherentes para análisis numéricos y de texto.

### Objetivo
El objetivo de este proceso de limpieza consiste en:

1. Manejo de valores faltantes: Identificar y tratar los valores faltantes en las columnas clave (stars, ratings).
2. Conversión de la columna 'price': Limpiar la columna price, eliminando comas, reemplazando valores como "Free" por 0, y convirtiendo los valores a formato numérico.
3. Transformación de texto: Mejorar la legibilidad de las columnas de texto como Author y Narrator, separando correctamente las palabras que están unidas por letras mayúsculas sin espacios intermedios.
4. Verificación de la limpieza: Mostrar las primeras filas de las columnas clave para verificar que la limpieza fue realizada correctamente.

### Funciones Implementadas
1. Manejo de valores faltantes: Se identificaron las columnas con valores faltantes, como stars y ratings. Se verificó la cantidad de valores nulos en cada columna y se decidió cómo manejarlos dependiendo del contexto.

2. Conversión de la columna price: Se reemplazaron valores como "Free" con 0 para tratar los productos gratuitos como cero. Se eliminaron las comas en los valores de price (por ejemplo, de "1,000" a "1000") para permitir una conversión adecuada a tipo numérico. Se convirtió la columna price a tipo flotante para análisis numérico.

3. Transformación de texto: Se usaron expresiones regulares para separar correctamente los nombres de Author y Narrator donde estaban escritos sin espacios intermedios.

4. Verificación de la limpieza: Se imprimieron las primeras filas de la columna price después de la limpieza para comprobar que los valores están en el formato correcto.

### Resultados Esperados
Al ejecutar el código, el archivo audible_data.csv será limpiado, con la columna price correctamente convertida a valores numéricos y las columnas de texto como Author y Narrator mejoradas. Se mostrará una vista previa de los primeros valores de las columnas clave para confirmar que la limpieza ha sido exitosa.

