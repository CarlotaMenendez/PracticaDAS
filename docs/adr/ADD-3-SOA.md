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

Chosen option: "[ADD-3. SOA]", because [trabaja en base a la integración de servicios, y para el problema estamos buscando independencia de los mismo. Además un fallo en el SOA afecta a todo el sistema.]

## Links

* [ADD-1](https://github.com/CarlotaMenendez/PracticaDAS/blob/main/docs/adr/ADD-1-Arquitectura-de-microservicios.md) [ADD-1-Arquitectura-de-microservicios.md]
* [ADD-2](https://github.com/CarlotaMenendez/PracticaDAS/blob/main/docs/adr/ADD-2-Cliente-servidor.md) [ADD-2-Cliente-Servidor.md]

<!-- markdownlint-disable-file MD013 -->
