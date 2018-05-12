# Arquitectura-Micro-Servicios
Repositorio de la tarea 2

## Sistema de Procesamiento de Comentarios

Antes de ejecutar el código asegurate de instalar los prerrequisitos del sistema ejecutando:
> sudo pip install -r requirements.txt

Los paquetes que se instalarán son los siguientes:

| Paquete  | Versión                             | Descripción |
| -------- | ----------------------------------- | ----------- |
| Flask    | 0.10.1                              | Micro framework de desarrollo |
| requests | 2.12.4                              | API interna utilizada en Flask para trabajar con las peticiones hacia el servidor |
| afinn    | 0.1                                 | API para realizar analisis de sentimientos |
| tweepy   | 3.6.0                               | API para recolectar los comentarios de Twitter |

*__Nota__: También puedes instalar éstos prerrequisitos manualmente ejecutando los siguientes comandos*
```sh
$ sudo pip install Flask
$ sudo pip install requests
$ sudo pip install afinn
$ sudo pip install tweepy
```


Una vez instalados los prerrequisitos es momento de ejcutar el sistema siguiendo los siguientes pasos:
1. Ejecutar el servicio:
   ```sh
   $ python servicios/sv_information.py
   $ python servicios/sv_tweets.py
   $ python servicios/sv_clasification.py
   ```
1. Ejecutar el GUI:
   ```sh
   $ python gui.py
   ```
1. Abrir el navegador
1. Acceder a la url del sistema:
   > http://localhost:8000/ - página de inicio!

Las especificaciones de los servicios se encuentran en servicios/README.md
*__Nota__: El proyecto trabaja con Python 2.7
