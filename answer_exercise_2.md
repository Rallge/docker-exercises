
## 2. [1 pto] Indica la diferencia entre el uso de la instrucción ADD y COPY (Dockerfile).

```bash
ADD 
- Se puede descargar y descomprimir.
- Ejemplo: ( 1 linea)
ADD https://github.com/dotcloud/docker/archive/master.tar.gz /root/

COPY
- Solo copia archivos y mas.
- Ejemplo: (2 lineas)

COPY master.tar.gz   /root
RUN  tar -xvf /root/master.tgz

- La diferencia es que que la instrucción COPY no permite ningún archivo fuera de contexto. Entonces, si está transmitiendo 
Dockerfile a través del archivo stdin o una URL (que no apunta a un código fuente repositorio), no se puede utilizar 
la instrucción COPY.
Ejemplo: Esto no se podria dar
COPY http://example.com/bar.go   /tmp/main.go 

```
