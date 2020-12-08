# [Comunicación asincrona entre los microservicios]

* Status: [Accepted]
* Deciders: [Alberto Jimenez, Manuel Martin, Javier Mendez]
* Date: [09/12/2020]

## Context and Problem Statement

[Se podrá utilizar una comunicación asíncrona realizada a través de un bus de eventos. Se implementará bien a través de un agente de mensajería (como RabbitMQ) o de un Service Bus (como Azure Service Bus), además servirá para propagar actuaizaciones entre microservicios.]

## Decision Drivers

* [driver 1, RF-15]
* [driver 2, RF-15.1]

## Considered Options

* [ADD-19] Patrón Mediator
* [ADD-20] Patrón de Bus

## Decision Outcome

Chosen option: "[Patrón de Bus]", because [Necesitamos una comunicación asincrona basada en un bus de eventos, y hemos decidido implementarlo mediante un bus Service bus (como por ejemplo Azure service bus) en vez de un agente de mensajería que además nos servirá para la propagación de actualizaciones].

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

### Pros and Cons of the Options

* Good, because [La comunicación entre objetos es encapsulada con un objeto mediador.]
* Good, because [Los objetos no se comunican de forma directa entre ellos, en lugar de ello se comunican mediante el mediador]
* Bad, because [Hay que crear un objeto mediador.]

## Links

* [ADD-19](https://github.com/CarlotaMenendez/PracticaDAS/blob/main/docs/adr/ADD-19-Patrón-Mediator.md) [ADD-19-Patrón-Mediator.md]

<!-- markdownlint-disable-file MD013 -->
