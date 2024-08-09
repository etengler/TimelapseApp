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

El **primer paso** para la instalación es **crear una cuenta de Gcloud**. Puede seguir este tutorial: [Tutorial-Cuenta-GCloud](https://github.com/etengler/TimelapseApp/blob/main/Tutorial%20-%20Cuenta%20GCloud.pdf)

Independiente del método elegido anteriormente, es importante obtener el **nombre del proyecto** para seguir con la instalación (guardarlo para un paso mas adelante).

&nbsp;
-----------------------------------------------------------------------------------------------------

El **segundo paso** es Descargar la carpeta TimelapseApp desde GitHub en **Code ----> Download ZIP**

![image](https://github.com/user-attachments/assets/316df2b0-cbeb-4411-ae77-d75211709a02)


&nbsp;

A continuación, pegar la descarga en una carpeta en nuestra pc y accedar hasta ver los archivos. Vamos a necesitar hacer dos cosas.

&nbsp;

Por un lado, **ABRIR** el archivo Timelapse.ipynb y **MODIFICAR** la linea **"ee.Initialize(project='...')"** con el nombre del proyecto. Se encuentra dentro de las primeras lineas del archivo. 


Por otro lado, vamos a necesitar **copiar** la ruta donde se encuentran los archivos para un paso más adelante.

![image](https://github.com/user-attachments/assets/570d53c2-f1d9-478e-99d8-62c6ab9a76cf)


&nbsp;
-----------------------------------------------------------------------------------------------------

El **tercer paso** es la **intsalación de los componentes** de la aplicación en nuestra PC. Será necesario jecutar las siguientes líneas en negrita.

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

##

Este código es una adaptación del que se encuentra disponible en el sitio web https://geemap.org/
