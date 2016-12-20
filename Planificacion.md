---
lang: es
title: Sistemas Operativos
author: Facultad de Ingeniería, Universidad de Buenos Aires
date: Primer cuatrimestre de 2017
linkcolor: black
urlcolor: blue
links-as-notes: false
header-includes: |
  \usepackage{draftwatermark}
  \SetWatermarkText{\textsc{Borrador}}
  \SetWatermarkColor[gray]{0.925}
---

# Resumen #

En la materia se estudia en detalle tres pilares fundamentales de los sistemas operativos:

  1. _compartición_ de recursos (procesador y memoria)

  2. acceso _concurrente_ (a recursos y datos)

  3. almacenamiento _persistente_ (de datos de usuario)

así como las abstracciones y conceptos subyacentes.

En los trabajos prácticos se ejercita tanto la implementación de dichas abstracciones como su uso a través de una interfaz de programación estándar.


# Objetivos #

Los objetivos se entroncan en torno a la idea del sistema operativo como _proveedor de servicios;_ así:

- Saber describir los servicios y funciones de un sistema operativo moderno.

- Conocer las abstracciones y detalles de implementación de dichos servicios, así como los algoritmos y estructuras asociados.

- Escribir programas que hagan uso de los servicios del sistema operativo a través de su interfaz de programación estándar.

- Implementar, sobre el núcleo de un sistema operativo existente, uno o más de estos servicios.


# Contenidos mínimos #

Funciones del sistema operativo. Procesos: creación y planificación. Espacio de direcciones; manejo de asignaciones; paginación. Hilos de ejecución y primitivas de sincronización. Organización de un sistema de archivos.


# Programa analítico #

**Unidad 1**

Sistemas operativos: propósito, funcionalidad y servicios. Historia breve y tipos. Separación de privilegios: ejecución del núcleo _(kernel)_ frente a código de usuario. Llamadas al kernel _(syscalls)_ como interfaz de acceso a servicios. Biblioteca del sistema y estándar POSIX.

**Unidad 2**

Compartición de procesador y memoria: el proceso como unidad de virtualización. Creación de procesos: paso de un archivo ejecutable a una instancia de proceso. Datos y estados de un proceso. Salto entre ejecución privilegiada _(kernel-space)_ y ejecución en nombre de un ususario _(user-space)_. Salto entre procesos de usuario.

Caso de estudio y práctica: intérprete de comandos _(shell)_ en un entorno POSIX.

**Unidad 3**

Espacios de direccionamiento y traducción de direcciones. Soporte hardware para traducción de direcciones. Paginación y TLB _(translation lookaside buffers)_. Caché, jerarquías de memoria y políticas de reemplazo.

Caso de estudio y práctica: manejador de memoria en espacio de usuario sobre la llamada al sistema _sbrk_.

**Unidad 4**

Planificación de procesos _(scheduling):_ orden de acceso al procesador. Estrategias básicas de planificación: _first-in first-out_ (FIFO), _shortest job first_ (SJF) y _shortest time-to-completion first_ (STCF); _round robin_ (RR) mediante tiempo de respuesta. Estrategias de repartición justas _(fair-share scheduling)_. Introducción a la planificación multi-procesador.

Caso de estudio y práctica: _schedulers_ en Linux.

**Unidad 5**

**Unidad 6**

Introducción al Concepto de Concurrencia. El Concepto de Thread. La Abstracción de Threads. El API de Threads. Creación de threads. Un Thread por dentro. Detalles de Implementación. I/O Asincrónica y programación dirigida por eventos. Locks:Idea Básica. Estructuras de Datos basadas en Locks. Sincronización del Acceso a Objetos Compartidos. Objetos Compartidos y Sincronización de Variables. Condition variables. Exclusión Mútua. Semaforos. Problemas Comunes de Concurrencia. Implementación de sincronización de objetos. Diseño e implementaciòn de objetos compartidos. Sincronización multi-objeto. Deadlock. Enfoques alternativos de sincronización.

**Unidad 7**

Introducción a los Sistemas de Archivos. La abstracción del Sistema de Archivos, El API del Sistema de Archivos. Capas de Software. Discos Magneticos. Redundant Array of Inexpensive Disks (RAID). Almacenamiento Flash. Archivos y Directorios. El API de Archivos. Archivos: localización y búsqueda de datos, Directorios: Poniendole nombre a los datos. FFS. Sistemas de archivos Alternativos.

**Unidad 8**

Seguridad. Sistemas Distribuidos. Sistemas Operativos Móviles. Sistemas Operativos de Tiempo Real.


# Bibliografía #


# Cronograma #


# Calendario de evaluaciones #


# Bibliografía #

- Anderson, T. y Dahlin, M.: _Operating Systems: Principles and Practice_ (2.ª ed.), Recursive Books (2014).

- Arpaci-Dusseau, R. H. y Arpaci-Dusseau, A. C.: _Operating Systems: Three Easy Pieces_ (v0.91), Arpaci-Dusseau Books (2015). [Disponible en línea en [ostep.org](http://ostep.org).]


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
