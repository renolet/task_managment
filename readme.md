# Task Manager web service

- Esta aplicación permite a los usuarios crear y mantener una lista de tareas, o sea que permite crear una tarea y eliminarla, se puede modificar sus datos como por ejemplo su estado puede ser eliminada, finalizada o cancelada. 
- Ademas permite que se realicen busquedas y filtrados mediante fecha de creación y/o contenido de la misma según título o descripción.



## Aspectos Técnicos:

- Este sistema es un RESTful web service, el cual esta desarrollado en lenguaje Python mediante la framework de Django y el uso fundamental de la herramienta Django REST framework.



## Instalación y uso:

- Clonar el repositorio a una carpeta de proyectos local.
- Migrar la base de datos: docker-compose run web python manage.py migrate
- Crear un usuario superuser con la instrucción: docker-compose run web python manage.py createsuperuser


## Objetivos:

El usuario de la aplicación tiene que ser capaz de:

- Crear una tarea
- Eliminar una tarea
- Marcar tareas como completadas
- Poder ver una lista de todas las tareas existentes
- Filtrar/buscar tareas por fecha de creación y/o por el contenido de la misma

