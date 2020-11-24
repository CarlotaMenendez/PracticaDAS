# [Bases de datos de microservicios]

* Status: [Accepted]
* Deciders: [Alberto Jimenez, Manuel Martín, David Mestanza, Javier Mendez]
* Date: [24/11/2020]

## Context and Problem Statement

[Para lograr la coherencia entre las bases de datos de los diferentes microservicios, usaremos eventos de integración de nivel de aplicación, así la comunicación entre microservicios es más flexible.]

## Decision Drivers

* [Driver 1, RF-11]
* [Driver 2, RF-11.1]

## Considered Options

* [ADD-5] Patrón CQRS.

## Decision Outcome

Chosen option: "[Patron CQRS]", because [ El patrón CQRS separa las operaciones de lectura y escritura de un almacen de datos, que usa comandos para actualizar los datos y consultas para leerlos.]

### Positive Consequences 

* [Escalado indepediente de las cargas de lectura y escritura.]
* [Consultas mas sencillas, la aplicación evita combinaciones complejas durnate las consultas.]
* [Asegura que solo escriban las entidades de dominio correctas.]
* [Como consequencia de la separación de lectura y escritura, se puede dar lugar a un modelo mas flexible y facil de mantener.]

### Negative Consequences 

* [Puede generar un diseño de aplicación mas complejo.]
* [Si se separa la base de datos de lectura y escritura, los datos pueden quedar obsoletos.]

<!-- markdownlint-disable-file MD013 -->
