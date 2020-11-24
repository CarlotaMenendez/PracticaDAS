# Logica de negocio y acceso a base de datos

* Status: [accepted] 
* Deciders: [Alberto Jimenez, Manuel Martin, Javier Mendez] 
* Date: [20/11/2020] 

## Context and Problem Statement

[Se necesita implementar una base de datos que almacene datos del mundo real y que estos datos puedan ser creados, cambiados y guardados]

## Decision Drivers 

* [driver 1: RF.-3]
* [driver 2, RF.-4]

## Considered Options

* [ADD-5] Patrón CQRS

## Decision Outcome

Chosen option: "[Patron CQRS]", because [ El patrón CQRS separa las operaciones de lectura y escritura de un almacen de datos, que usa comandos para actualizar los datos y consultas para leerlos.  ].

### Positive Consequences 

* [Escalado indepediente de las cargas de lectura y escritura]
* [Consultas mas sencillas, la aplicación evita combinaciones complejas durnate las consultas]
* [Asegura que solo escriban las entidades de dominio correctas]
* [Como consequencia de la separación de lectura y escritura, se puede dar lugar a un modelo mas flexible y facil de mantener]

### Negative Consequences 

* [Puede generar un diseño de aplicación mas complejo]
* [Si se separa la base de datos de lectura y escritura, los datos pueden quedar obsoletos]

<!-- markdownlint-disable-file MD013 -->
