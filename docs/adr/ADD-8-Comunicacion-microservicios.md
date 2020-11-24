# [Comunicación entre microservicios]

* Status: [accepted]
* Deciders: [Alberto Jimenez, Manuel Martin, David Mestanza, Javier Mendez]
* Date: [24/11/2020]

## Context and Problem Statement

[Los microservicios independientes se deben de comunicar entre ellos de forma independente a través del protocolo REST y de forma asíncrona. ]

## Decision Drivers

* [driver 1, RF-9]

## Considered Options

* [ADD-Y] Patrón Mediator

## Decision Outcome

Chosen option: "[Patrón Mediator]", because [estamos buscando que los microservicios sean independientes y no dependan unos de otros. Con este patrón conseguimos justo eso, que se comuniquen consiguiendo toda la independecia evitando problemas a futuro].

### Positive Consequences

* [La comunicación entre objetos es encapsulada con un objeto mediador.]
* [Los objetos no se comunican de forma directa entre ellos, en lugar de ello se comunican mediante el mediador.]
* [Reduce las dependencias entre los objetos en comunicación.]

### Negative Consequences

* [Hay que crear un objeto mediador.]

<!-- markdownlint-disable-file MD013 -->
