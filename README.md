# CODIFICADOR DE COORDENADAS EN ARCHIVOS PLANOS

## INTRODUCCIÓN

> Una de las aplicaciones desarrolladas por WAWANDCO utiliza información de ubicación geográfica para generar valor comercial para uno de sus clientes. Esta aplicación genera archivos de registro (sin formato) en el dispositivo móvil del usuario que son útiles para depurar la información de los usuarios.

>Además de la información de ubicación geográfica, estos archivos planos contienen otra información relacionada con la aplicación.

>La solución ofrecida permite acceder a la información contenida en dicho archivo plano y extraer los datos relacionados con la ubicación (coordenadas) para emitirlos finalmente a través de una polilínea codificada para los fines que se requieran

## ¿Cómo lo hace?
>
1.  La solución recibe la ruta donde se encuentra alojado el archivo plano
2.  Inicia la lectura del archivo
3. Busca coincidencias de un patrón de referencia en el texto
4. Almacena las coordenadas encontradas (sin repetirlas)
5. Procesa las coordenadas almacenadas y las prepara para su codificación
6. Finalmente codifica todas las coordenadas y las retorna a través de polilínea


## EJECUCIÓN

> El proceso de ejecución es bastante sencillo, en la ruta donde se encuentra este .MD, se encuentra también un ejecutable llamado solución que se puede ejecutar mediante la consola de comandos accediendo  a el desde dicha ruta,

>
1. Abrir la consola de comando 
2. Acceder a la ruta donde se encuentra el ejecutable
3. Lanzar el ejecutable (escribiendo su nombre simplemente)
4. una vez iniciada la ejecución, la solución pedirá un archivo plano para evaluar
5. Se debe indicar la ruta del archivo ejemplo: (C:\Users\Admin\Desktop\archivo.log)
6. Una vez se analice el archivo y se realice el proceso, la solución devolverá una polilínea codificada con todas las coordenadas encontradas en el archivo (sin repetirlas)


>Nota: Para ejecutar solution.go a través del comando "go run", es necesario que exista la carpeta "polyline" la cual debe contener el archivo polyline.go y (esta carpeta se debe encontrar en la misma ruta que solution.go)
