                                            --- TIMELAPSE --- 
                                                            
### Esta herramienta permite generar un **TIMELAPSE** de una región y un período en particular a partir de imágenes Landsat.

Con la selección de ciertos parámetros podrás generar un archivo en formato .gif o .mp4 que es posible descargar. 

&nbsp;

Este algoritmo utiliza librerías de código abierto como GeeMap que consume Google Earth Engine (GEE) para procesar y generar imágenes satelitales. 
El proceso de selección de imágenes es partir de la primera de cada año que cumpla con los parámetros de calidad.

&nbsp;

Es necesario el programa **Anaconda** o **Minianaconda** para ejecutarlo (Link de descarga: https://docs.anaconda.com/miniconda/)

Los pasos para la instalación y ejecución de la aplicación se presentan a continuación.


&nbsp;

                                          --- Interfaz visual --- 

<p align="center">
  <img src=images/timelapse.png alt="Interfaz">
</p>

&nbsp;

                                             --- Resultado --- 
                                                          
<p align="center">
  <img src=images/landsat_rioBermejo.gif alt="Gif">
</p>



&nbsp;


                                             --- Instalación ---

El **primer paso** es crear una cuenta en Google Earth Engine, en caso de no tener una. Link a Google Earth Engine: https://earthengine.google.com/

Una vez hecho esto, será necesario guardar el nombre del proyecto personal que se encuentra en el borde superior derecho de la pagina, como indica la flecha roja.

![image](https://github.com/user-attachments/assets/0d42ec22-373b-4142-9dcb-4ef9a1746928)

&nbsp;
-----------------------------------------------------------------------------------------------------

El **segundo paso** es descargar la carpeta TimelapseApp desde GitHub en **Code ----> Download ZIP**

![image](https://github.com/user-attachments/assets/316df2b0-cbeb-4411-ae77-d75211709a02)

&nbsp;

A continuación, guardar la descarga en una carpeta en nuestra pc y accedar hasta ver los archivos (flecha azul). Vamos a necesitar hacer dos cosas para poder hacer uso de la aplicación TIMELAPSE. 

![image](https://github.com/user-attachments/assets/dc74dd67-76e4-4f1d-919a-d2f6d164a575)

&nbsp;

Por un lado, **ABRIR** el archivo timelapse.ipynb y **MODIFICAR** la linea **"ee.Initialize(project='...')"** con el nombre de tu proyecto. Se encuentra dentro de las primeras líneas del archivo (flecha roja). 

![image](https://github.com/user-attachments/assets/dc1ca3e7-e16f-43ab-8c3d-ff13986e7366)


Por otro lado, vamos a necesitar **COPIAR** la ruta donde se encuentran los archivos (flecha verde) para un paso más adelante.

&nbsp;
-----------------------------------------------------------------------------------------------------

El **tercer paso** es la **intsalación de los componentes** de la aplicación en nuestra PC. Será necesario ejecutar los siguientes pasos en orden (texto en negrita).


  1- Abrir la consola de Anaconda o Minianaconda. 

  2- Pararse en la carpeta contenedora del proyecto: **cd ruta\donde\estan\los\archivos** (acá va la ruta mencionada mas arriba con la flecha verde)
  
  3- Crear el entorno virtual con todas las dependecias utilizadas: **conda env create --file ENV.yml**

  4- Activar el entorno virtual: **conda activate env_time**

  5- Otorgar permisos: **earthengine authenticate**
  
  6- Cerrar la consola.

  
&nbsp;

                       --- Ejecutar la aplicación TIMELAPSE ---

Una vez instalado, cada vez que se quiera ejecutar la aplicación, se deberán ejecutar los siguientes pasos:

  1- Abrir la consola de Anaconda o Minianaconda. 

  2- Acceder a la carpeta contenedora del proyecto:  **cd ruta\donde\estan\los\archivos** (acá va la ruta mencionada mas arriba con la flecha verde)

  3- Activar el entorno virtual: **conda activate env_time**

  4- Ejecutar la aplicación: **voila timelapse.ipynb**

Listo!

&nbsp;
----------------------------------------------------------------------------------------------------------------  


Este código es una adaptación del que se encuentra disponible en el sitio web https://geemap.org/

© 2024 Autor. Licensed under the Apache License 2.0.


