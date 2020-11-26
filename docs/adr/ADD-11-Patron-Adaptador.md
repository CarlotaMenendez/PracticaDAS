# [Soporte de tareas en la nueva arquitectura]

* Status: [rejected]
* Deciders: [Alberto Jimenez, Manuel Martin, David Mestanza, Javier Mendez]
* Date: [26/11/20220]

## Context and Problem Statement

[¿Como podemos trasladar las tareas de indentificación de usuarios, catálogo de microservicios y procesado de pedidos a una arquitectura de microservicos?
Podemos utilizar el patron visitor para acceder a las tareas con una clase externa y así no tener que tocar por dentro esas tareas pero aun asi manteniendo la opcion de añadir nuevas operaciones a nuestras tareas.]

## Decision Drivers

* [driver 1, RF-8]

## Considered Options

* [ADD-11] Patrón Adaptador
* [ADD-12] Patrón Visitor

## Decision Outcome

Chosen option: "[Patrón Adaptador]", because [queremos poder comunicarnos con las clases de las tareas pero no queremos meternos dentro de las propias clases para ello ].

## Links

* [ADD-12](https://github.com/CarlotaMenendez/PracticaDAS/blob/main/docs/adr/ADD-12-Patrón-Visitor.md) [ADD-12-Patrón-Visitor.md]


<!-- markdownlint-disable-file MD013 -->
