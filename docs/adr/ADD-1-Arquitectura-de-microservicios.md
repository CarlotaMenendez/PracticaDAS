# [Elección arquitectura de microservicios]

* Status: [accepted] 
* Deciders: [Alberto Jimenez, Manuel Martin, David Mestanza, Javier Mendez] 
* Date: [20/11/2020]

## Context and Problem Statement

[Una tienda virtual está basada en una arquitectura monolítica y se desea migrar a una arquitectura de microservicios más flexible y escalable.]

## Decision Drivers

* [Driver 1: La tienda utiliza microservicios independientes para realizar cada una de sus funciones, las cuales trabajan de forma asíncrona e independiente.]
* [Driver 2: La comunicación entre los microservicios se realiza mediante recurso ligeros como APIs de recursos HTTP.]

## Considered Options

* [ADD-1] Arquitectura de microservicios
* [ADD-2] Cliente-Servidor
* [ADD-3] SOA

## Decision Outcome

Chosen option: "[Arquitectura de microservicios]", because [es un método de desarrollo de aplicaciones software que funciona como un conjunto de pequeños servicios que se ejecutan de manera independiente y autónoma, proporcionando una funcionalidad de negocio completa y nos facilita la integración de aplicaciones de terceros y la independencia entre ellas.].

### Positive Consequences
* [Versátil, los microservicios permiten el uso de diferentes tecnologías y lenguajes. ]
* [Es fácil de integrar y escalar con aplicaciones de terceros. ]
* [Las soluciones desarrolladas con arquitectura de microservicio permiten la mejora rápida y continua de cada funcionalidad. ]
* [El mantenimiento es más simple y barato. ]

### Negative Consequences

* [Nos dificulta el testing. ]
* [Los tiempos de respuesta de distintos microservicios suelen ser más elevados. ]
* [Los desarrolladores tienen que tener especial cuidado con las comunicaciones entre los microservicios. ]

## Pros and Cons of the Options

### [ADD-2. Cliente-Servidor]

* Good, because [centralización del control aumentando la seguridad.]
* Bad, because [con una demanda muy alta por parte de los clientes podría caerse el servidor.]
* Bad, because [necesitaríamos de tener un hardware y software específico para albergar el servidor.]

### [ADD-3. SOA]

* Good, because [la orientación a servicios permite desarrollar aplicaciones con independencia de las plataformas y lenguajes de programación que realizan los procesos. ]
* Bad, because [trabaja en base a la integración de servicios. ]
* Bad, because [un fallo en el SOA afecta a todo el sistema. ]

## Links

* [ADD-2](https://github.com/CarlotaMenendez/PracticaDAS/blob/main/docs/adr/ADD-2-Cliente-servidor.md) [ADD-2-Cliente-Servidor.md]
* [ADD-3](https://github.com/CarlotaMenendez/PracticaDAS/blob/main/docs/adr/ADD-3-SOA.md) [ADD-3-SOA.md]

<!-- markdownlint-disable-file MD013 -->
