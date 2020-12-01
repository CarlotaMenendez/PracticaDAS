# [Encapsulación de microservicos en contenedores madiante el patrón Module]

* Status: [accepted]
* Deciders: [Alberto Jimenez, Manuel Martin, David Mestanza, Javier Mendez]
* Date: [01/12/2020]

## Context and Problem Statement

[El sistema necesitará utilizar contenedores para meter dentro los microservicios, accederemos a estos contenedores mediante hosts.
Esto se hará gracias al patrón Module que nos permitira juntar todos los elementos de un microservicio en un mismo contenedor facilitando asi una gran cantidad de procesos dentro de un mismo contenedor]

## Decision Drivers

* [driver 1, RF-13]

## Considered Options

* [ADD-15] Patrón Module

## Decision Outcome

Chosen option: "[Patrón Module]", because [queremos que cada contenedor contenga todos los elementos exclusivos del microservicio que tengamos dentro, así cuando estemos realizando cambios a un microservicio sabremos cuales son los elementos con los que tenemos que tener mas cuidado en vez de tener en cuenta todo el sistema con cada modificacion de un microservicio especifico].

### Positive Consequences

* [Encuapsula todos los elementos de un microservicio]
* [Facilita la comunicación entre todos los elementos de un mismo microservicio]
* [Simplifica la depuración despues de un cambio en cualquier microservico]

### Negative Consequences

* [Dificulta la comunicación entre dos elementos secundarios de microservicios distintos]

<!-- markdownlint-disable-file MD013 -->

