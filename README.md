                                            --- TIMELAPSE --- 
                                                            
## Esta herramienta permite generar un TIMELAPSE de una región y un período en particular a partir de imágenes Landsat.

Se necesita el programa **Anaconda** o **Minianaconda** para ejecutarlo (Link de descarga: https://docs.anaconda.com/miniconda/)

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

El **primer paso** es **crear una cuenta de Gcloud** para que la aplicación funcione.

Puede seguir este tutorial: [Tutorial-Cuenta-GCloud](https://github.com/etengler/TimelapseApp/blob/main/Tutorial%20-%20Cuenta%20GCloud.pdf)

&nbsp;

Independiente del método elegido anteriormente, es importante obtener el **nombre del proyecto** para seguir con la instalación.
Luego, se debe modificar la linea del archivo aguaTierra.ipynb

&nbsp;

El **segundo paso** es la **intsalación de los componentes** de la aplicación en nuestra PC. Es importante tener en cuenta que hay pasos que sólo se realizan por única vez y otros que deben ejecutarse cada vez que se desee utilizar la aplicación.

&nbsp;

                          --- Primera instalación ---

Serie de pasos a realizar por única vez la primera vez que se instala la aplicación. 

&nbsp;


A) Descargar la carpeta TimelapseApp desde GitHub en **Code ----> Download ZIP**

![image](https://github.com/user-attachments/assets/316df2b0-cbeb-4411-ae77-d75211709a02)

&nbsp;

B) Pegar la descarga en una carpeta en nuestra pc, accedar hasta ver los archivos y copiar esa ruta.

![image](https://github.com/user-attachments/assets/313fabe5-3aea-4eaf-afa4-abbca6af93de)

&nbsp;

C) Abrir la consola de Anaconda o Minianaconda. Ejecutar las siguientes líneas (en negrita):

   
  1- Abrir la consola de Anaconda o Minianaconda. 
  
  2- Acceder a la carpeta contenedora del proyecto: **cd ruta\donde\estan\los\archivos**
  
  3- Crear el entorno virtual con todas las dependecias utilizadas: **conda env create --file ENV.yml**

  4- Activar el entorno virtual: **conda activate env_time**

  5- Ejecutar la aplicación: **voila aguaTierra.ipynb**

  6- Otorgar permisos: **earthengine authenticate**

  7- Inicilaizar el proyecto. Aca es **IMPORTANTE** colocar el nombre del proyecto personal obtenido en el paso 1: 
    
  **python -c "import ee; ee.Initialize(project='ACA_VA_EL_NOMBRE_DEL_PROYECTO_DEL_PASO_1')"**

  8- Ejecutar la aplicación: **voila aguaTierra.ipynb**
  

&nbsp;

                       --- Pasos a realizar para ejecutar la aplicación (siempre y cuando se haya realizado el paso anterior) ---


  1- Abrir la consola de Anaconda o Minianaconda. 

  2- Acceder a la carpeta contenedora del proyecto:  **cd ruta\donde\estan\los\archivos**

  3- Activar el entorno virtual: **conda activate env_time**

  4- Ejecutar la aplicación: **voila aguaTierra.ipynb**


&nbsp;
----------------------------------------------------------------------------------------------------------------  

##

Este código es una adaptación del que se encuentra disponible en el sitio web https://geemap.org/
