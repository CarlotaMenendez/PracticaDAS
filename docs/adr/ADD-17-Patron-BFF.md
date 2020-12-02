# [Comunicación entre clientes y microservicios]

* Status: [accepted]
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

Chosen option: "[Patrón BFF]", because [nos permite considerar que el acceso a nuestro servicio se realiza desde clientes específicos con necesidades específicas, permite evolucionar las diferentes capas de la aplicación de manera paralela y elimina acoplamiento entre clientes diferentes con casos de uso específicos, siempre y cuando podamos asumir los costes de tener diferentes puntos de entrada a nuestra aplicación mantenidos por diferentes equipos].

### Positive Consequences

* [Problemas de seguridad, sin una puerta de enlace, todos los microservicios deben estar expuestos al mundo externo.]
* [Cada microservicio publicado públicamente debe abordar inquietudes como la autorización, SSL, etc. En muchas situaciones, esas preocupaciones podrían manejarse en un solo nivel para que los microservicios internos se simplifiquen.]
* [Un cliente puede requerir varias llamadas a multiples microservicios, la agregación manejada a un nivel intermedio, podría mejorar el rendimiento y la experiencia del usuario para la aplicación cliente. ]
* [Elimina acoplamiento entre clientes diferentes con casos de uso específicos]
* [Es mas facil que un servicio de backend evolucione, ya que las adaptaciones no necesitarán cambios en el cliente, solo en los adaptadores]


### Negative Consequences

* [Puede añadir mucha complejidad al sistema]
* [La complejidad tambien aumenta el coste, más hardware, más configuración y un encarecimiento del  desarrollo]
* [Requiere que los equipos de cliente tengan capacidad para generar su propio servicio de backend, lo que implica tener conocimientos de backend en un equipo frontend o un equipo mobile]

### Pros and Cons of the Options

[ADD- Patrón de puerta de enlace API]

* Good, because [ Tiene las mismas ventajas de tener una puerta de enlace API, pero simplificando la complejidad y bajando el coste.]
* Bad, because [No elimina el acoplamiento entre clientes diferentes con casos de uso especifico al tener solamente una unica puerta de enlace API, lo cual tambien puede crear un único punto de error adicional.]

## Links

* [ADD-16](https://github.com/CarlotaMenendez/PracticaDAS/blob/main/docs/adr/ADD-16-Patron-Puerta-Enlace-API.md) [ADD-16-Patron-Puerta-Enlace-API]

<!-- markdownlint-disable-file MD013 -->
