# Docker - Servidor Web (NGINX)

Bootcamp para la creación de un servidor Web NGINX básico

## Descargar una imagen NGINX y ejecutarla
```
docker container run nginx
```
## Ejecución del servidor NGINX
```
docker container run --name my-nginx -p 80:80 nginx
```
## Listando los contenedores actuales
```
docker container ls
```
## Detener el contenedor
```
docker container stop my-nginx
```
## (Re)Iniciar el contenedor
```
docker container start my-nginx
```
## Sesión interactiva
```
docker run --name docker-nginx-01 -p 80:80 -d nginx
docker exec -it 90c5b531d19b bash
```
# Mi primer sitio Web
* Revisar el archivo ```Dockerfile```
* Revisar la página inicial ```index.html```

Crear la imagen a partir del Dockerfile:
```
docker build -t simple-nginx .
docker images
```
Ejecutar la imagen en consola:
```
docker run -it -p 8080:80  --rm --name simple-nginx-running-app simple-nginx
```
# Borrar todo
## Detener el contenedor y luego borrarlo:
```
docker container stop my-nginx
docker container remove my-nginx
```

## Borrar la imagen
```
docker image remove nginx
```

