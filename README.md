                                            --- TIMELAPSE --- 
                                                            
## Esta herramienta permite generar un TIMELAPSE de una región y un período en particular a partir de imágenes Landsat.

Es necesario el programa **Anaconda** o **Minianaconda** para ejecutarlo (Link de descarga: https://docs.anaconda.com/miniconda/)

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

El **primer paso** es crear una cuenta en Google Earth Engine, en caso de no tener una. 

Link de Google Earth Engine: https://earthengine.google.com/

Una vez hecho esto, será necesario guardar el nombre del proyecto que se encuentra en el borde superior derecho de la pagina, como indica la flecha roja.

![image](https://github.com/user-attachments/assets/0d42ec22-373b-4142-9dcb-4ef9a1746928)

&nbsp;
-----------------------------------------------------------------------------------------------------

El **segundo paso** es descargar la carpeta TimelapseApp desde GitHub en **Code ----> Download ZIP**

![image](https://github.com/user-attachments/assets/316df2b0-cbeb-4411-ae77-d75211709a02)

&nbsp;

A continuación, guardar la descarga en una carpeta en nuestra pc y accedar hasta ver los archivos (flecha azul). Vamos a necesitar hacer dos cosas para poder hacer uso de la aplicación TIMELAPSE. 

![image](https://github.com/user-attachments/assets/12e56a08-3d71-4cd2-8f03-60002b8a3a65)

Por un lado, **ABRIR** el archivo Timelapse.ipynb y **MODIFICAR** la linea **"ee.Initialize(project='...')"** con el nombre del proyecto. Se encuentra dentro de las primeras líneas del archivo. 

![image](https://github.com/user-attachments/assets/b6fbc916-36d9-4b48-b57b-e570a9cd9328)

Por otro lado, vamos a necesitar **COPIAR** la ruta donde se encuentran los archivos (flecha verde) para un paso más adelante.

&nbsp;
-----------------------------------------------------------------------------------------------------

El **tercer paso** es la **intsalación de los componentes** de la aplicación en nuestra PC. Será necesario ejecutar los siguientes pasos en orden (texto en negrita).

&nbsp;

  1- Abrir la consola de Anaconda o Minianaconda. 

  2- Pararse en la carpeta contenedora del proyecto: **cd ruta\donde\estan\los\archivos**
  
  3- Crear el entorno virtual con todas las dependecias utilizadas: **conda env create --file ENV.yml**

  4- Activar el entorno virtual: **conda activate env_time**

  5- Otorgar permisos: **earthengine authenticate**
  
  6- Cerrar la consola.

  
&nbsp;

                       --- Ejecutar la aplicación TIMELAPSE ---

Una vez instalado, cada vez que se quiera ejecutar la aplicación, se deberán ejecutar los siguientes pasos:


  1- Abrir la consola de Anaconda o Minianaconda. 

  2- Acceder a la carpeta contenedora del proyecto:  **cd ruta\donde\estan\los\archivos**

  3- Activar el entorno virtual: **conda activate env_time**

  4- Ejecutar la aplicación: **voila aguaTierra.ipynb**


&nbsp;
----------------------------------------------------------------------------------------------------------------  


Este código es una adaptación del que se encuentra disponible en el sitio web https://geemap.org/
