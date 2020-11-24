# [Cesta de compra]

* Status: [accepted]
* Deciders: [Alberto Jimenez, Manuel Martin, David Mestanza, Javier Mendez]
* Date: [24/11/2020]

## Context and Problem Statement

[Función cesta de compra para que el cliente pueda almacenar varios productos en la caché y así pueda continuar comprando en vez de tener que comprar producto a producto, y una vez finalizada su compra pueda hacerla toda de una, comprando así varios productos a la vez.]

## Decision Drivers

* [Driver 1, RF-10]

## Considered Options

* [ADD-X] MongoDB

## Decision Outcome

Chosen option: "[MongoDB]", because [MongoDB guarda estructuras de datos BSON (una especificación similar a JSON) con un esquema dinámico, haciendo que la integración de los datos en ciertas aplicaciones sea más fácil y rápida.].

### Positive Consequences

* [Código fuente abierto y disponible para varios sistemas operativos.]
* [Cualquier campo en un documento de MongoDB puede ser indexado, al igual que es posible hacer índices secundarios.]
* [Balanceo de carga.]

### Negative Consequences

* [Problemas de escalabilidad: el rendimiento baja cuando se opera con más de 100GB.]
* [MongoDB bloquea la base de datos a nivel de documento ante cada operación de escritura]

<!-- markdownlint-disable-file MD013 -->
