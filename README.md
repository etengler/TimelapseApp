                                            --- TIMELAPSE --- 
                                                            
## Esta herramienta permite generar un TIMELAPSE de una región y un período en particular a partir de imágenes Landsat.

Se necesita Anaconda para ejecutarlo.

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

Pasos: 

1) Pegar los archivos en una carpeta en nuestra pc. Luego, acceder a esa carpeta desde la consola de Anaconda.

    **cd ruta\donde\estan\los\archivos**

 
2) A continuación, ejecutar las siguientes líneas en orden:

    conda env create --file ENV.yml

    **conda activate env_time**

    earthengine authenticate
    (deberá otorgar permisos)

    **voila aguaTierra.ipynb**

Este último paso abrirá el navegador con la aplicación!!

&nbsp;

La línea "conda env create --file ENV.yml" que crea el entorno virtual, y "earthengine authenticate" deben ejecutarse sólo una única vez. La siguiente vez que desee usar la aplicación esos pasos no serán necesarios ya que el entorno ya estará creado y ya se ha autenticado! Es decir, se deben ejecutar todos los pasos excepto esos.

&nbsp;   

##


Este código es una adaptación del que se encuentra disponible en el sitio web https://geemap.org/
