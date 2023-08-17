# Docker - Servidor Web (NGINX)

Bootcamp para la creación de un servidor Web NGINX básico

## Descargar una imagen NGINX

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




