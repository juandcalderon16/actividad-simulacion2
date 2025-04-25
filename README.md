# Actividad de seguimiento - Simulación 2

|Integrante|correo|usuario github|
|---|---|---|
|Juan Diego Calderon Bermeo|juand.calderon@udea.edu.co|juandcalderon16|
|Ana Maria Vega Angarita|ana.vega@udea.edu.co|anavegaa|

## Instrucciones

Antes de empezar a realizar esta actividad haga un **fork** de este repositorio y sobre este trabaje en la solución de las preguntas planteadas en la actividad de simulación. Las respuestas deben ser respondidas en español o si lo prefiere en ingles en el lugar señalado para ello (La palabra **answer** muestra donde).


## Homework (Simulation)

This program, [mlfq.py](mlfq.py), allows you to see how the MLFQ scheduler presented in this chapter behaves. See the [README](https://github.com/remzi-arpacidusseau/ostep-homework/blob/master/cpu-sched-mlfq/README.md) for details.


### Questions

1. Run a few randomly-generated problems with just two jobs and two queues; compute the MLFQ execution trace for each. Make your life easier by limiting the length of each job and turning off I/Os.

2. How would you run the scheduler to reproduce each of the examples in the chapter?
   
   Para configurar el simulador de MLFQ para que se comporte como
 un planificador Round-Robin, debemos asegurarnos de que todos los trabajos 
tengan el mismo nivel de prioridad, que el tiempo de quantum sea el mismo para todas las colas, y que no 
haya ningún tipo de boost que altere las prioridades.


   `./mlfq.py -n 1 -q 10 -a 1 -j 2 -m 20 -M 1000 -i 5 -c`

   Este comando ejecuta una simulación con un solo trabajo (de tipo Round-Robin) que tiene un quantum de 10 unidades de tiempo y una asignación de 1 rebanada de tiempo por cola. Se generarán dos trabajos, cada uno con un máximo de 20 unidades de tiempo de tiempo de ejecución y una frecuencia de I/O muy baja (1000 unidades de tiempo). Además, las solicitudes de I/O tomarán 5 unidades de tiempo cada una.


3. How would you configure the scheduler parameters to behave just like a round-robin scheduler?

   <details>
   <summary>Answer</summary>
   Coloque aqui su respuerta
   </details>
   <br>

4. Craft a workload with two jobs and scheduler parameters so that one job takes advantage of the older Rules 4a and 4b (turned on
with the -S flag) to game the scheduler and obtain 99% of the CPU over a particular time interval.

   <details>
   <summary>Answer</summary>
   Coloque aqui su respuerta
   </details>
   <br>

5. Given a system with a quantum length of 10 ms in its highest queue, how often would you have to boost jobs back to the highest priority level (with the `-B` flag) in order to guarantee that a single longrunning (and potentially-starving) job gets at least 5% of the CPU?

   <details>
   <summary>Answer</summary>
   Coloque aqui su respuerta
   </details>
   <br>

6. One question that arises in scheduling is which end of a queue to add a job that just finished I/O; the -I flag changes this behavior
for this scheduling simulator. Play around with some workloads and see if you can see the effect of this flag.

   <details>
   <summary>Answer</summary>
   Coloque aqui su respuerta
   </details>
   <br>

## Conclusions

Coloque aqui las conclusiones...


### Criterios de evaluación
- [x] Despligue de los resultados y analisis claro de los resultados respecto a lo visto en la teoria.
- [x] Creatividad y orden.
- [x] Sección con las conclusiones de los experimentos realizados.
