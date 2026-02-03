Bandit – Reporte de Progreso

Objetivo general:
Resolver los niveles del wargame Bandit encontrando las contraseñas de cada nivel mediante la exploración de archivos y directorios, 
utilizando distintos comandos de la línea de comandos en Linux.

Nivel 0
Se estableció una conexión SSH al servidor Bandit y se listaron los archivos del directorio personal. La contraseña se encontraba en un archivo de texto visible.

Nivel 1
Se identificó un archivo con un nombre especial que podía interpretarse como una opción de comando, por lo que fue necesario especificar su ruta explícitamente.

Nivel 2 
Se localizó un archivo cuyo nombre contenía espacios. Para poder acceder a él, se utilizaron comillas al momento de leer el archivo.

Nivel 3
Se ingresó a un directorio específico y se listaron todos los archivos, incluidos los ocultos, para identificar el archivo que contenía la información requerida.

Nivel 4
Se encontraron múltiples archivos y se utilizó el comando file para identificar cuál de ellos contenía texto legible, descartando los archivos binarios.

Nivel 5
Se utilizó el comando find para localizar un archivo que cumpliera con ciertas condiciones como tamaño, permisos y tipo.

Nivel 6
Se realizó una búsqueda a nivel del sistema usando find, filtrando por usuario, grupo y tamaño del archivo.

Nivel 7
Se utilizó el comando grep para buscar una línea específica que contenía una palabra clave dentro de un archivo extenso.

Nivel 8
El archivo contenía múltiples líneas duplicadas y solo una línea única. Para identificarla, se ordenó el contenido del archivo y se filtraron las líneas que aparecían una sola vez.

Nivel 9
El archivo no contenía texto legible directamente, por lo que se utilizó el comando strings para extraer cadenas de texto. Posteriormente, se filtraron los resultados para localizar la información relevante.

Nivel 10
El contenido del archivo se encontraba codificado en Base64, por lo que fue necesario decodificarlo para poder leer la información original y obtener la contraseña.
