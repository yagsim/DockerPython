# Docker + python 

---
## Creamos un contenedor sencillo de python  
    $ docker run -it --rm --name my-running-script -v "$PWD":/usr/src/myapp -w /usr/src/myapp python:3 python your-daemon-or-script.py

 ``docker``     el comando base 
 
``ru``    crear el contenedor
 
``-it``      dos opciones que valen para i=interactuar con el contenedor y t= con la terminal
 
``--rm``     borra el contenedor cuando lo termina de usar

 ``-v``     define el mapeo del volumen 
 
- ``$PWD`` el directorio donde estamos   ((en windows ruta absoluta))

- ``/usr/src/myapp``   directorio dentro del contenedor

``-w``    el directorio de trabajo(_workdir_)

``python:3``   la imagen de la que se creara el contenedor

``python your-daemon-or-script.py``   comando para ejecutar dentro del contenedor

