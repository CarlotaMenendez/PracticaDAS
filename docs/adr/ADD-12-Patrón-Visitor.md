# [Soporte de tareas en la nueva arquitectura madiante el patrón Visitor]

* Status: [accepted]
* Deciders: [Alberto Jimenez, Manuel Martin, David Mestanza, Javier Mendez]
* Date: [26/11/2020]

## Context and Problem Statement

[¿Como podemos trasladar las tareas de indentificación de usuarios, catálogo de microservicios y procesado de pedidos a una arquitectura de microservicos?
Podemos utilizar el patron visitor para acceder a las tareas con una clase externa y así no tener que tocar por dentro esas tareas pero aun asi manteniendo la opcion de añadir nuevas operaciones a nuestras tareas.]

## Decision Drivers

* [driver 1, RF-8]

## Considered Options

* [ADD-11] Patrón Adaptador
* [ADD-12] Patrón Visitor

## Decision Outcome

Chosen option: "[Patrón Visitor]", because [queremos poder comunicarnos con las clases de las tareas pero no queremos meternos dentro de las propias clases para ello, por lo que utilizando la clase Visitor accederemos a las clases de las tareas].

### Positive Consequences

* [Permite el acceso a las tareas sin modificar nada de las clases en sí]
* [Deja abierta la posibilidad de añadir nuevas operaciones de forma sencilla]

### Negative Consequences

* [Nos dificulata añadir nuevas clases para otras tareas que no sean las tres que tenemos]

## Pros and Cons of the Options

### [Patrón Adaptador]

Nos permite acceder a las tareas sin preocuparnos por el formato de las funciones y variables.

* Good, because [Facil de implementar]
* Bad, because [Nos dificulta modificar las funciones de las tareas y implementadas]
* Bad, because [Nos dificulta añadir operaciones nuevas a las tareas]


## Links

* [ADD-11](https://github.com/CarlotaMenendez/PracticaDAS/blob/main/docs/adr/ADD-11-Patron-Adaptador.md) [ADD-11-Patrón-Adaptador.md]

<!-- markdownlint-disable-file MD013 -->
