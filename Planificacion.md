---
lang: es
---

# Objetivos #

**Objetivos generales**

- Conocer, estudiar y describir los objetivos, servicios, mecanismos y funciones de un sistema operativo moderno. Estos se dividen en 4 bloques fundamentales:

    1. Kernel y procesos.

    2. Administración de memoria.

    3. Concurrencia.

    4. Persistencia.

- Obtener las habilidades necesarias para programar a nivel kernel mediante la ejercitación sobre un sistema operativo concreto.

- Conocer, estudiar y describir otros conceptos relacionados con los sistemas operativos modernos (seguridad, tolerancia a fallos, tiempo real y evaluación de performance, etc.)

- Conocer, utilizar e implementar las herramientas más comunes que proveen los sistemas operativos modernos.


**Objetivos particulares**

- Conocer, estudiar y utilizar los algoritmos y estructuras de datos más utilizados en la contrucción de sistemas operativos modernos.


- Conocer, comprender y aplicar las soluciones que normalmente se aplican a los problemas que se presentan en un sistema operativo moderno.


# Contenidos mímimos #

Kernel y procesos. Administración de memoria. Concurrencia. Persistencia.


# Programa sintético #

Núcleos (kernels) y procesos. La abstracción del núcleo (kernel). La interfase de programación. Administracion de memoria. Memoria real, memoria virtual y memoria caché. Aplicaciones de administración de memoria. Concurrencia y threads. Sincronización de acceso a objetos compartidos. Algoritmos de scheduling. Sistemas de archivos. Dispositivos de almacenamiento. Archivos y directorios.


# Programa Analítico #

**Unidad 1**

Introducción. Qué es un Sistema Operativo. Criterios de Evaluación de un Sistema Operativo. Historia de los Sistemas Operativos. Tipos de Sistemas Operativos.

**Unidad 2**

La abstracciòn del Kernel. El concepto de Proceso. La abstracción del Proceso. Estados de un Proceso. Estruturas de datos. Modo de Operación dual. Transferencia de control segura. Caso de estudio: Booteando un kernel de un sistema operativo. Caso de Estudio: Maquinas Virtuales.

**Unidad 3**

El API de Procesos. Gestión de Procesos. Input/Output. Caso de Estudio: Implemención de un shell. Caso de Estudio: Comunicación Interproceso. Estructura de un sistema Operativo.

**Unidad 4**

Memoria Física. La Abstracción del Espacio de Memoria. El API de Memoria. El Concepto de Espacio de Direcciones. Paginación. Algoritmos de Paginación. Segmentación. Administración de Espacio Libre de Memoria.  Software address translation.  Memoria Caché. El Concepto de Cache. Gestión de memoria Cache. Memoria Virtual VAX / VMS.

**Unidad 5**

Introducción a la Planificación. Planificación Uniprocesador. Planificación Multiprocesador. Planificación Energy-aware. Planificación de Tiempo Real. Teoria de Colas. Caso de estudio.

**Unidad 6**

Introducción al Concepto de Concurrencia. El Concepto de Thread. La Abstracción de Threads. El API de Threads. Creación de threads. Un Thread por dentro. Detalles de Implementación. I/O Asincrónica y programación dirigida por eventos. Locks:Idea Básica. Estructuras de Datos basadas en Locks. Sincronización del Acceso a Objetos Compartidos. Objetos Compartidos y Sincronización de Variables. Condition variables. Exclusión Mútua. Semaforos. Problemas Comunes de Concurrencia. Implementación de sincronización de objetos. Diseño e implementaciòn de objetos compartidos. Sincronización multi-objeto. Deadlock. Enfoques alternativos de sincronización.

**Unidad 7**

Introducción a los Sistemas de Archivos. La abstracción del Sistema de Archivos, El API del Sistema de Archivos. Capas de Software. Discos Magneticos. Redundant Array of Inexpensive Disks (RAID). Almacenamiento Flash. Archivos y Directorios. El API de Archivos. Archivos: localización y búsqueda de datos, Directorios: Poniendole nombre a los datos. FFS. Sistemas de archivos Alternativos.

**Unidad 8**

Seguridad. Sistemas Distribuidos. Sistemas Operativos Móviles. Sistemas Operativos de Tiempo Real.


# Bibliografía #

- Anderson, Thomas; Dahlin, Michael: _Operating Systems: Principles and Practice_, Recursive Books (2.ª ed., 2012).

- Arpaci-Dusseau, Remzi H.; Arpaci-Dusseau, Andrea C.: _Operating Systems: Three Easy Pieces_, Arpaci-Dusseau Books (v0.91, 2015).


# Régimen de cursada #

**Metodología de enseñanza**

Resolución por parte de los alumnos y controlada por los docentes auxiliares de problemas correspondientes a
las unidades temáticas del programa, ya sea por escrito o por máquina (programas). En general se tratará
de problemas abiertos, que generen dudas y motiven la consulta a los docentes y la profundización del
conocimiento a través de la bibliografía. Durante el curso se plantearán trabajos prácticos con problemas
complejos a resolver por programación, que los alumnos deberán desarrollar en grupo

**Modalidad de Evaluación Parcial**
De manejo de conceptos, aplicación de conocimientos y dominio de técnicas, mediante la respuesta a
preguntas y la resolución de problemas por escrito en evaluaciones parciales e integradoras, y el desarrollo
controlado de trabajos prácticos en computadora.
Las evaluaciones parciales e integradoras son por unidades o subunidades temáticas.
La evaluación de los trabajos por computadora es por presentación en tiempo y forma (plazos y formato
establecido), método de desarrollo (aplicación de método de desarrollo)

# Calendario de clases #

Semana         | Temas de  Teoria                       | Resolucion de problemas
------------   | -------------                          | -------------
Clase 1: 10/3  |  Introducción                          |
Clase 2: 17/3  |La abstracción Kernel                   |  Caso de Estudio
Clase 3: 24/3  |La abstracción de Proceso               |
               |El Api de Procesos                      |  Caso de Estudio
Clase 4: 31/3  |Introducción a la Planificación.        |
               |Planificación Uniprocesador.            |
               |Planificación Multiprocesador.          |
               |Planificación Energy-aware.             |
               |Planificación de Tiempo Real.           |
               |Teoria de Colas.                        | Caso de estudio
Clase 5: 7/4   | La Abstracción del Espacio de Memoria  |
               | El API de Memoria                      |
Clase 6: 14/7   | El Concepto de Espacio de Direcciones  |
               | Paginación. Algoritmos de Paginación   |
Clase 7: 21/4  | Segmentación. Memoria Caché.           |
               |El Concepto de Cache.                   |
Clase 8: 28/4   |Introducción al Concepto de Concurrencia|
               |El API de Threads. Creación de threads. |
               |El Concepto de Thread                   |
Clase 9: 5/5     |La Abstracción de Threads.              |
               |Un Thread por dentro. Detalles de Implementación. |
Clase 10: 12/5  |Locks:Idea Básica.                      |
               |Objetos Compartidos y Sincronización de Variables. |
               |Estructuras de Datos basadas en Locks.   |
               |Condition variables. Exclusión Mútua. Semaforos. |
Clase 11: 19/5   |Problemas Comunes de Concurrencia.       |
               |Sincronización multi-objeto. Deadlock.   |
Clase 12: 26/5  |La abstracción del Sistema de Archivos   |
               |El API del Sistema de Archivos           |
Clase 13: 9/6   |Sistemas de Archivos. Archivos. Directorios|
Clase 14: 16/6  |                              | 1er Parcial
Clase 15: 23/6   |Segutidad                     |
               |Sistemas Distribuidos        |
Clase 16: 30/6 |             | 1er Recuperatorio del Parcial



# Calendario de evaluaciones #

1er Parcial semana 14
1er recuperatorio semana 16
2do recuperatorio  Oportunidad fuera del período de clases 1er semana de finales
