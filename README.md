# Tan Proyect
 
<<<<<<< HEAD
## Informacion acerca de las librerias/frameworks/plugins utilizadas en Front-end, Back-end y Base de datos
### VUE.js : Framework en javascript en el que desarrollamos todo el frontend
#### Axios : Nuestra libreria para la comunicacion http y requests ajax
#### Vuex : libreria para almacenar componentes de nuestra app
#### Bootstrap : framework para nuestro frontend que facilita el desarrollo de html y css
#### Router : libreria para manejar nuestras Rutas

## Frontend
-flask : Framework principal con el que hacemos la aplicacion
=======
# Informacion acerca de las librerias/frameworks/plugins utilizadas en Front-end, Back-end y Base de datos
-vue: framework utilizado para la creación del frontend
>>>>>>> 
-datetime : Para guardar los posts con la fecha de creacion.
-wtforms : Validadores de email, longitud, data requerida, etc para los formularios
-PIL : Para la compresion de imagenes que se usan en los perfiles
-secrets : Para generar una cadena de caracteres aleatorios para serializar
-os : Para usar algunas variables de entorno y unos path para las imagenes

# El nombre del script a ejecutar para iniciar la base de datos con datos
## Backend:
desde la carpeta de TanDBP
### CMD: 
cd TanDBP para acceder a la carpeta
set flask_app = server
set flask_env = development
flask run

# Informacion acerca de los API. Requests y Responses de cada endpoint utilizado en el sistema.
## Rutas del backend:
/users -> GET : Para obtener el json con los usuarios
/signup -> GET, POST : Para añadir un nuevo usuario
/users -> POST : Para añadir un nuevo usuario (version DEPRECADA de prueba para postman)
/user -> GET : Peticion de prueba para validar un token
/login -> GET, POST : Para pasar los datos del usuario y mediante jwt obtener el token

# Hosts
Frontend VUE.js : Localhost Puerto: 3000
Backend Flask : Localhost Puerto : 5000
# Forma de autenticacion
Usamos JWT para autenticar a los usuarios. Todos los usuarios son creados con un public_id que es creado usando un identficador universal, en nuestro caso usamos el uuid4, y la clave es hasheada por la libreria werkzeug usando el sha256 el cual es un hash cryptografico bastante popular desarrollado por la seguridad nacional de Estados Unidos.
Cuando un usuario se loguea e ingresa tanto su usuario como contraseña, este pasa por el encabezado de autorizacion en la solicitud y nuestro backend primero busca que el usuario exista, luego desencripta la contraseña y comprueba que sea valida para finalmente usando el json web token, retorne un token unico que dura 30 minutos hecho con nuestra secret key. 


# Errores HTTP:
- 500: Lo utilizamos para cuando se genera algun error en el servidor
- 404: En caso el cliente trate de acceder a una ruta inexistente
- 403: En caso el cliente trate de acceder a una ruta a la que no tiene permisos para acceder
- 422: El servidor esta recibiendo la peticion sin embargo hay algun error que esta haciendo que la peticion sea improcesable.
- 200: OK (caso de exito)
