# *ARSW - Laboratorio 2*
# Programación concurrente, condiciones de carrera, esquemas de sincronización, colecciones sincronizadas y concurrentes.
## Integrantes:

- Eduard Arias
- James Torres

## *Descripción* 
Este ejercicio tiene como fin que el estudiante conozca y aplique conceptos propios de la programación concurrente en el caso de Dogs Race.

## *PARTE I*
Creación, puesta en marcha y coordinación de hilos.

1. Revise el programa “primos concurrentes” (en la carpeta parte1), dispuesto en el paquete edu.eci.arsw.primefinder. Este es un programa que calcula los números primos entre dos intervalos, distribuyendo la búsqueda de los mismos entre hilos independientes. Por ahora, tiene un único hilo de ejecución que busca los primos entre 0 y 30.000.000. Ejecútelo, abra el administrador de procesos del sistema operativo, y verifique cuantos núcleos son usados por el mismo.

EL programa utiliza un maximo de 2 nucleos para la ejecucion. 

![Ejecución del programa](./img/media/lab/image2.png) 