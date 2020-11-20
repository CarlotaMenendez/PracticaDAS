# [Eleccion de arquitectura]

* Status: [rejected]
* Deciders: [Alberto Jimenez, Manuel Martin, David Mestanza, Javier Mendez]
* Date: [20/11/20220]

## Context and Problem Statement

[Una tienda virtual está basada en una arquitectura monolítica y se desea migrar a una arquitectura de microservicios más flexible y escalable.]

## Decision Drivers

* [Driver 1: La tienda utiliza microservicios independientes para realizar cada una de sus funciones, las cuales trabajan de forma asíncrona e independiente.]
* [Driver 2: La comunicación entre los microservicios se realiza mediante recurso ligeros como APIs de recursos HTTP.]

## Considered Options

* [ADD-1. Arquitectura de microservicios]
* [ADD-2. Cliente-Servidor]
* [ADD-3. SOA]

## Decision Outcome

Chosen option: "[ADD-2. Cliente-Servidor]", because [necesitaríamos software y hardware específico que supondría un gasto que no estamos dispuestos a correr. Además al tener tantos servicios simultáneos es fácil que se caiga el servidor.]

## Links <!-- optional -->

* [Link type] [Link to ADR] <!-- example: Refined by [ADR-0005](0005-example.md) -->
* … <!-- numbers of links can vary -->

<!-- markdownlint-disable-file MD013 -->
