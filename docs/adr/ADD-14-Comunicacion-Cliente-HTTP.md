# [Comunicación de cliente a través de HTTP]

* Status: [accepted]
* Deciders: [Alberto Jimenez, Manuel Martin, David Mestanza, Javier Mendez]
* Date: [01/12/2020]

## Context and Problem Statement

[Los clientes podrán comunicarse con el microservicio de HTTP a través de un Gateway que contiene diversas APIs con el fin de poder consultar las actualizaciones desde las aplicaciones cliente.]

## Decision Drivers

* [Driver 1, RF-14]

## Considered Options

* [ADD-14] Patrón API Gateway centralizado on-premise y en la nube.

## Decision Outcome

Chosen option: "[Patrón API Gateway centralizado on-premise y en la nube]", because [es un modelo que consiste en utilizar ambos patrones de despliegue; es decir, dos clusters independientes. Para consumo interno, sobre todo si hay temas legales involucrados, se opta por la implantación on-premise y para el consumo externo la implantación en la nube, en concreto, se utilizan versiones SaaS del producto en caso de que se tengan.]

### Positive Consequences

* [Alto rendimiento.]
* [Implementación rápida.]
* [Multiplataforma y flexibilidad de uso.]
* [Conectividad efectiva.]
* [Requisitos legales y seguridad.]

### Negative Consequences

* [Mantenimiento y gestión más compleja]
* [Personal dedicado con conocimiento del producto.]

<!-- markdownlint-disable-file MD013 -->
