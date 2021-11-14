# [MPWAR] – Entorno Web
Entregable 1

## 1. [1 pto] Indica la diferencia entre el uso de la instrucción CMD y ENTRYPOINT
(Dockerfile).

```bash
CMD
- CMD especifica los argumentos que se pasan al ENTRYPOINT (para argumentos)
- No hay un CMD por defecto en docker.
- CMD establece comandos y / o parámetros predeterminados, que se pueden sobrescribir desde la línea de comandos
cuando se ejecuta el contenedor Docker.

ENTRYPOINT
- ENTRYPOINT especifica un comando que siempre se ejecutará cuando se inicie el contenedor. 
- Docker tiene por defecto el ENTRYPOINT ["bin/sh","-c"].
- El comando ENTRYPOINT y los parámetros no se sobrescribirán desde la línea de comando. En cambio, todos los 
argumentos de la línea de comandos se agregarán después de los parámetros ENTRYPOINT.
```
