# [Comunicación cliente-microservicios]

* Status: [accepted]
* Deciders: [Alberto Jimenez, Manuel Martin, David Mestanza, Javier Mendez]
* Date: [02/12/2020]

## Context and Problem Statement

[Una vez tengamos listos los microservicios estos deberán comunicarse con las aplicaciones clientes, concretamente a través del uso de contenedores. Además estos deberán usar direcciones URL públicas publicadas con las puertas de enlace API.]

## Decision Drivers

* [driver 1, RF-16]

## Considered Options

* [ADD-18] Patrón Mediator

## Decision Outcome

Chosen option: "[Patrón Mediator]", because [estamos buscando la comunicación entre aplicaciones cliente y microservicios. Estos se harán a través de contenedores en unas determinadas circunstancias. Estos contenedores serán nuestros objetos mediadores, y es por eso por lo que escogemos este patrón].

### Positive Consequences

* [La comunicación entre objetos es encapsulada con un objeto mediador.]
* [Los objetos no se comunican de forma directa entre ellos, en lugar de ello se comunican mediante el mediador.]
* [Reduce las dependencias entre los objetos en comunicación.]

### Negative Consequences

* [Hay que crear los contenedores en base a unas especificaciones.]

<!-- markdownlint-disable-file MD013 -->
