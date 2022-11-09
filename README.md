# Actividad 1 - Construcción de imágenes Docker y despliegue con Docker Compose (laboratorio)

## Objetivos


Node.js es un entorno de ejecución de Javascript diseñado para crear aplicaciones escalables, el cual sigue un modelo asíncrono y dirigido por eventos. Por otro lado, los ficheros Dockerfile nos proporcionan una manera declarativa y consistente de construir imágenes de Docker para nuestras aplicaciones.

Esta actividad consiste en «contenerizar» una sencilla aplicación existente de Node.js en una imagen de Docker mediante un fichero Dockerfile. Una vez generada la imagen, desplegaremos la aplicación en contenedores a partir de un fichero de Docker Compose. Además, nuestra aplicación de ejemplo requiere de una base de datos MongoDB, por lo que deberemos desplegarla también en un contenedor.

Algunas consideraciones:

- Al generar la imagen con Dockerfile deberemos instalar las dependencias de la aplicación necesarias con el gestor de paquetes npm, y exponer el puerto 3000. Además, se deberán seguir las buenas prácticas recomendadas.

- En el fichero de Docker Compose se deberán definir el servicio de la aplicación Node.js y el de la base de datos MongoDB. La conexión a la base de datos en la aplicación está definida en el fichero db.js.

- Los contenedores deberán estar conectados a través de una red especifica de Docker y la aplicación deberá ser accesible en el puerto 3000.

- Una vez este desplegada la aplicación y ejecutándose correctamente, obtenga los logs de los contenedores desplegados.

- Por último, publique en Docker Hub la imagen generada. Si no dispone de usuario, puede crearse una cuenta de manera gratuita.
