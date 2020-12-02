# [Comunicación entre clientes y microservicios]

* Status: [rejected]
* Deciders: [Alberto Jimenez, Manuel Martin, David Mestanza, Javier Mendez]
* Date: [02/12/2020]

## Context and Problem Statement

[los clientes móviles y de páginas Web se comunicarán con los puntos de conexión
de puerta de enlace de API única y, a continuación, se comunicarán con los microservicios. Los clientes web tradicionales se comunicarán con el microservicio MVC, que se comunicará con otros microservicios mediante la puerta de enlace de API.]

## Decision Drivers

* [driver 1, RF-12]
* [driver 2, RF-12.1]

## Considered Options

* [ADD-16] Patrón de puerta de enlace API
* [ADD-17] Patrón BFF

## Decision Outcome

Chosen option: "[Patrón de puerta de enlace API]", because [Este es un servicio que proporciona un punto de entrada único para ciertos grupos de microservicios, se parece al patrón facade pero forma parte de un sistema distribuido].

### Positive Consequences

* [Problemas de seguridad, sin una puerta de enlace, todos los microservicios deben estar expuestos al mundo externo.]
* [Cada microservicio publicado públicamente debe abordar inquietudes como la autorización, SSL, etc. En muchas situaciones, esas preocupaciones podrían manejarse en un solo nivel para que los microservicios internos se simplifiquen.]
* [Un cliente puede requerir varias llamadas a multiples microservicios, la agregación manejada a un nivel intermedio, podría mejorar el rendimiento y la experiencia del usuario para la aplicación cliente. ]

### Negative Consequences

* [Una puerta de enlace de API exige un mayor desarrollo y mantenimiento futuro si incluye lógica personalizada y agregación de datos.]
* [Usar una puerta de enlace de API de microservicios crea un posible único punto de error adicional]
* [Si no se escala horizontalmente de manera correcta, la puerta de enlace de API puede dar lugar a un cuello de botella]

## Links

* [ADD-17](https://github.com/CarlotaMenendez/PracticaDAS/edit/main/docs/adr/ADD-17-Patron-BFF.md) [ADD-17-Patron-BFF]

<!-- markdownlint-disable-file MD013 -->
