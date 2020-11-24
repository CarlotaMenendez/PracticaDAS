# Logica de integración de aplicaciones

* Status: [Accepted] 
* Deciders: [Alberto Jimenez, Manuel Martin, Javier Mendez, David Mestanza] 
* Date: [24/11/2020] 

## Context and Problem Statement

[Se necesita implementar un canal de mensajeria entre aplicaciones , principalmente mediante agentes de mensajeria]

## Decision Drivers 

* [driver 1: RF.-5]

## Considered Options

* [ADD-6] Patrón Mediator

## Decision Outcome

Chosen option: "[Patron Mediator] ", because [ necesitamos un canal de mensajeria en el que las aplicaciones se comuniquen independientemente y con este patrón conseguimos justo esto, evitando problemas en el futuro ].

### Positive Consequences 

* [La comunicación entre objetos es encapsulada con un objeto mediador.]
* [Los objetos no se comunican de forma directa entre ellos, en lugar de ello se comunican mediante el mediador.]
* [Reduce las dependencias entre los objetos en comunicación.]

### Negative Consequences 

* [Hay que crear un objeto mediador.]

<!-- markdownlint-disable-file MD013 -->
