# [Integración de microservicios]

* Status: [accepted]
* Deciders: [Alberto Jimenez, Manuel Martin, David Mestanza, Javier Mendez]
* Date: [25/11/2020]

## Context and Problem Statement

[Buscamos la forma en que la aplicación pueda integrar microservicios de forma asíncrona para aumentar la fiabilidad y seguridad de los microservicios nativos de la tienda virtual. Estos microservicios deberán ser independientes.]

## Decision Drivers

* [driver 1, RF-6]

## Considered Options

* [ADD-10] Patrón de Bus

## Decision Outcome

Chosen option: "[Patrón de Bus]", because [El patrón de bus cumple con todo el contexto de los drivers, nos da la independencia de los microservicios con el desacople, y la seguridad de los ya existentes. Además nos da otra gran variedad de funciones y mejoras.].

### Positive Consequences

* [Desacoplamiento: en un escenario típico de fuerte acoplamiento tenemos toda una red de conexiones punto a punto entre las mismas. Con el uso de un patrón bus que desacople a las aplicaciones tendremos un esquema similar a este: Las aplicaciones no se relacionan directamente entre sí.]
* [Adaptación de protocolo y formato: mediante el bus de integración, al ser una pieza intermedia que se coloca entre el cliente del servicio y el proveedor del mismo, puede realizar el trabajo de adaptación de formatos de datos y protocolos.]
* [Configuración y no programación: normalmente los patrones de bus se acompañan de herramientas de desarrollo que hacen énfasis en reducir lo máximo posible la codificación. En su lugar, proporcionan un entorno visual en el que las tareas o acciones a realizar se representan con cajas unidas por flechas que indican el flujo de los datos.]
* [Control de errores: cada backend tendrá su propia manera de representar un error. Con la capa de patrones de bus de integración es posible tener un punto centralizado donde gestionar estos errores y además proporcionar al cliente un interfaz único de estos errores.]
* [Securización: podemos establecer un modo de securización común y homogéneo para los diferentes backends que pueden tener una securización muy diferente.]

### Negative Consequences

* [Posibilidad de desborde al recibir muchos paquetes de datos.]
* [Potencial imprevisión de escalabilidad.]
* [No hay mucho soporte de recuperación en caso de falla parcial. Una vez el bus cae, puede colgar el resto de acciones de usuario.]

<!-- markdownlint-disable-file MD013 -->
