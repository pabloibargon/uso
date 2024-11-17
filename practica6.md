# Práctica 6: Gestión de procesos

1. Compara la salida de `ps` con `ps -ef`.

2. Crea un proceso en segundo plano que simplemente espere durante 1 hora. Prueba que puedes seguir usando la terminal con otro comando.

3. Busca en `ps -ef` la información del proceso que acabas de crear. (No lo busques a mano ...)

4. Lista los procesos del usuario `root`.

5. _Mata_ el proceso del apartado 2 haciendo uso de so PID. Comprueba que ya no aparece en el listado de `ps`.

6. Crea otro proceso similar y repite lo mismo haciendo uso de su identificador como trabajo.

7. Repite con `kill -15`, `kill -SIGTERM`, `kill -9`, `kill -SIGKILL`, interpreta estas variaciones.

8. Crea un proceso que escriba "Terminado" después de 10 segundos. Páralo con [CTRL+Z], ejecuta `bg` para reanudar el proceso. Comprueba que puedes seguir usando la terminal con otro comando. Comprueba que finalmente se escribe "Terminado".

9. Crea un proceso que escriba "Terminado" después de 10 segundos. Páralo con [CTRL+Z], ejecuta `fg` para reanudar el proceso. Comprueba que NO puedes seguir usando la terminal con otro comando. Comprueba que finalmente se escribe "Terminado".

10. Realmente [CTRL+Z] envía otro tipo de señal, `SIGSTOP`. Crea un proceso EN SEGUNDO PLANO que escriba "Terminado" después de 30 segundos. Envía esta señal al proceso mediante su PID y comprueba que no se escribe "Terminado". Finaliza reanudándolo.

# BONUS: Descarga de ficheros

11. Muestra estas preguntas, que se encuentran subidas en la ruta `https://raw.githubusercontent.com/pabloibargon/uso-p6/refs/heads/main/practica6.md` usando el comando `curl`.

12. Prueba ahora con el comando `wget`. Explica la diferencia en el comportamiento por defecto de `wget` y `curl`.

13. Consigue descargarlo a un fichero con `curl` usando la opción -o.