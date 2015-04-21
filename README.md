# Django

## PASOS
1.- Crea la carpeta del proyecto en donde tendras el virtualenv y el projecto en django.

hecto932 [10:29 PM]
2.- Entra al directorio creado y crea el Virtualenv con virtualenv venv, donde venv es el nombre de la carpeta donde se instalara el entorno virtual

hecto932 [10:29 PM]
3.- Activas el virtualenv primeramente (sin sudo) source venv/bin/activate

hecto932 [10:30 PM]
4.- Ahora que tienes el Virtualenv corriendo debes instalar django y pillow(Yo lo hice al mismo tiempo)
pip install django y pip install pillow, sin sudo

hecto932 [10:31 PM]
5.- Creamos un proyecto django-admin.py startproject <nombre_del_proyecto>

hecto932 [10:34 PM]
6.- A partir de Django 1.7.5 South viene por defecto asi que el siguiente paso va a ser ./manage.py migrate, con esto vamos a poder crear todas las tablas iniciales que necesitamos para llevar el control de versiones de nuestras bases de datos

hecto932 [10:35 PM]
7.- Creamos todos nuestros modulos como dice harvey: tracks, albums, artists

hecto932 [10:36 PM]
8.- Creamos los campos en cada modulo y  agregamos los modulos en settings.py

hecto932 [10:37 PM]
8.- hacemos ./manage.py makemigrations que lo que hace es preparar todos los cambios en nuestros modelos para su posterior migracion

hecto932 [10:37 PM]
9 **

hecto932 [10:38 PM]
10 .- Aplicamos la migracion preparada con ./manage.py migrate y se creara en cada modelo las tablas de bases de datos que se llevan hasta ese momento

hecto932 [10:38 PM]
11.- Por ultimo podemos hacer ./manage.py syncdb para crear un usuario de backend para el administrador de Django

hecto932 [10:39 PM]
Con el cual puedes entrar haciendo http://127.0.0.1:8000/admin/