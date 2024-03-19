                                                          --- TIMELAPSE --- 
                                                            
## Esta herramienta permite generar un TIMELAPSE de una región y un período en particular a partir de imágenes Landsat.

Se necesita Anaconda para ejecutarlo.

&nbsp;

                                                      --- Interfaz visual --- 

<p align="center">
  <img src=images/timelapse.png alt="Interfaz">
</p>

                                                          --- Resultado --- 
                                                          
<p align="center">
  <img src=images/landsat_rioBermejo.gif alt="Gif">
</p>



&nbsp;

En Anaconda se deberá ejecutar la siguiente manera: 

1) Pegar los archivos en una carpeta en nuestra pc. Luego, acceder a esa carpeta desde la cosnola de Anaconda.

 cd ruta\donde\estan\los\archivos

 
2) A continuacion correr las siguientes lineas en orden uno por uno:

    conda env create --file ENV.yml

    conda activate ENV

    voila aguaTierra.ipynb
   

##


Este código es una adaptación del que se encuentra disponible en el sitio web https://geemap.org/
