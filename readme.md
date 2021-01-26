# Task Manager web service

- Esta aplicación permite a los usuarios llevar a cabo la gestión y mantenimiento de listas de tareas, o sea que permite crear y eliminar tareas, permite mostrar todas las tareas o una en particular, permite poder modificar sus datos y además cambiar su estado pudiendo tomar uno de los siguientes: Activa, Finalizada o Cancelada. 
- Ademas permite que se realicen busquedas y filtrados mediante fecha de creación y/o contenido de la misma según título o descripción.



## Aspectos Técnicos:

- Este sistema es un RESTful web service, el cual esta desarrollado en lenguaje Python mediante la framework de Django y el uso fundamental de la herramienta Django REST framework.



## Instalación y uso:

Para poder correr el proyecto es necesario seguir los siguientes pasos:

- Clonar el repositorio a una carpeta de proyectos local.
- Pararse en la rama "master".
- Migrar la base de datos: docker-compose run web python manage.py migrate
- Crear un usuario superuser el cual nos va a permitir poder gestionar las tareas. Para crearlo usar la instrucción: docker-compose run web python manage.py createsuperuser 
- Correr el servior local mediante: docker-compose up
- Importar la colección de postman que se encuentra en la carpeta "postman" para poder correr los endpoints.
- Obtener token del superuser mediante el request que se encuentra en Postman en Account/Account Token. Previamente cambiar los datos de usuario y password por los del usuario recientemente creado.
- En la carpeta "Tarea" de Postman se encuentran todos los requests necesarios para el llamado a los endpoints correspondientes a Tareas. 


## Test:

Esta aplicación contiene un set de pruebas unitarias fundamentalmente para testear los endpoints para la gestión de tareas. Para poder realizar el test correr la siguiente instrucción:

- docker-compose run web python manage.py test


