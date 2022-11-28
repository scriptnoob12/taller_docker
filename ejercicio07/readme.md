## Ejercicio 07- Taller Docker

Se estan ejecutando dos contenedores.
EL primer contenedor esta basada en la imagen nicopaez/jobvacancy-ruby:1.3.0
El segundo contenedor esta basado en postgres:14.4-alphine



version: hace referencia a la version del docker compose
services: indica los contenedores ej: web y db
	
image: indica la imagen base
links: indica al contenedor que esta enlazado
ports: indica el puerto a utilizar
environment: indica las variables de entorno
depends_on: indica de que contenedores depende este contenedor
	

	
