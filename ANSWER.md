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

![Ejecución del programa](./img/media/lab/2.PNG) 

2. Modifique el programa para que, en lugar de resolver el problema con un solo hilo, lo haga con tres, donde cada uno de éstos hará la tarcera parte del problema original. Verifique nuevamente el funcionamiento, y nuevamente revise el uso de los núcleos del equipo.

- Se realizó la modificación incluyendo casos de borde.

![Actualización de programa](./img/media/lab/3.PNG)

3. Lo que se le ha pedido es: debe modificar la aplicación de manera que cuando hayan transcurrido 5 segundos desde que se inició la ejecución, se detengan todos los hilos y se muestre el número de primos encontrados hasta el momento. Luego, se debe esperar a que el usuario presione ENTER para reanudar la ejecución de los mismo.

- Para detener un hilo en Java se utiliza su método 'stop()', pero está deprecado (al menos desde java 11)

![Detener ejecución después de 5 segundos](./img/media/lab/4.PNG)


## *PARTE II*