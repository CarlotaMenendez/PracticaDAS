# [short title of solved problem and solution]

* Status: [proposed] <!-- optional -->
* Deciders: [Alberto Jimenez, Manuel Martin, David Mestanza, Javier Mendez] <!-- optional -->
* Date: [18/11/2020] <!-- optional -->

## Context and Problem Statement

[Una tienda virtual está basada en una arquitectura monolítica y se desea migrar a una arquitectura de microservicios más flexible y escalable.]

## Decision Drivers <!-- optional -->

* [Driver 1: La tienda utiliza microservicios independientes para realizar cada una de sus funciones, las cuales trabajan de forma asíncrona e independiente.]
* [Driver 2: La comunicación entre los microservicios se realiza mediante recurso ligeros como APIs de recursos HTTP.]
* … <!-- numbers of drivers can vary -->

## Considered Options

* [ADD-1. Arquitectura de microservicios]
* [ADD-2. Cliente-Servidor]
* [ADD-3. SOA]
* … <!-- numbers of options can vary -->

## Decision Outcome

Chosen option: "[ADD-1. Arquitectura de microservicios]", porque [es un método de desarrollo de aplicaciones software que funciona como un conjunto de pequeños servicios que se ejecutan de manera independiente y autónoma, proporcionando una funcionalidad de negocio completa y nos facilita la integración de aplicaciones de terceros y la independencia entre ellas.].

### Positive Consequences <!-- optional -->

* [Versátil, los microservicios permiten el uso de diferentes tecnologías y lenguajes. ]
* [Es fácil de integrar y escalar con aplicaciones de terceros. ]
* [Las soluciones desarrolladas con arquitectura de microservicio permiten la mejora rápida y continua de cada funcionalidad. ]
* [El mantenimiento es más simple y barato. ]

### Negative Consequences <!-- optional -->

* [Nos dificulta el testing. ]
* [Los tiempos de respuesta de distintos microservicios suelen ser más elevados. ]
* [Los desarrolladores tienen que tener especial cuidado con las comunicaciones entre los microservicios. ]

## Pros and Cons of the Options <!-- optional -->

### [option 1]

[example | description | pointer to more information | …] <!-- optional -->

* Good, because [argument a]
* Good, because [argument b]
* Bad, because [argument c]
* … <!-- numbers of pros and cons can vary -->

### [option 2]

[example | description | pointer to more information | …] <!-- optional -->

* Good, because [argument a]
* Good, because [argument b]
* Bad, because [argument c]
* … <!-- numbers of pros and cons can vary -->

### [option 3]

[example | description | pointer to more information | …] <!-- optional -->

* Good, because [argument a]
* Good, because [argument b]
* Bad, because [argument c]
* … <!-- numbers of pros and cons can vary -->

## Links <!-- optional -->

* [Link type] [Link to ADR] <!-- example: Refined by [ADR-0005](0005-example.md) -->
* … <!-- numbers of links can vary -->

<!-- markdownlint-disable-file MD013 -->
