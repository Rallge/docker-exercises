## 3. [2,5 ptos] Crea un contenedor con las siguientes especificaciones:

* Utilizar la imagen base NGINX haciendo uso de la versión 1.19.3
* Al acceder a la URL localhost:8080/index.html aparecerá el mensaje HOMEWORK 1
* Persistir el fichero index.html en un volumen llamado static_content
Nota: Adjuntar una breve explicación de todos los pasos que has seguido para la
consecución de los objetivos marcados en el enunciado y todos los
comandos/ficheros utilizados

Los archivos usados para este ejercicio esta guardado en este repositorio. Carpeta: static_content

PASO 1:
Descargamos la imagen de docker de la versión 1.19.3

```bash
docker pull nginx:1.19.3
```
PASO 2:
Crear un archivo index.html dentro de la carpeta *static_content* que sera el nombre de nuestro volumen

PASO 3:
Debemos de estar dentro de la carpeta static_content para luego escribir el siguiente comando para ejecutar el contenedor 
some-nginx en el puerto 8080 y se levantará el contenedor mostrando el mensaje HOMEWORK 1 
y ejecutandose en una versión de nginx:1.19.3

```bash
 docker run -d -p 80:80 --name some-nginx -v $(PWD):/usr/share/nginx/html:ro -d nginx:1.19.3
```
