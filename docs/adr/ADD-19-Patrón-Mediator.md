# Comunicación asincrona entre microservicios

* Status: [rejected] 
* Deciders: [Alberto Jimenez, Manuel Martin, Javier Mendez] 
* Date: [09/12/2020] 

## Context and Problem Statement

[Se podrá utilizar una comunicación asíncrona realizada a través de un bus de eventos. Se implementará bien a través de un agente de mensajería (como RabbitMQ) o de un Service Bus (como Azure Service Bus), además servirá para propagar actuaizaciones entre microservicios.]

## Decision Drivers 

* [driver 1: RF-15]
* [driver 1: RF-15.1]

## Considered Options

* [ADD-19] Patrón Mediator
* [ADD-20] Patrón de Bus

## Decision Outcome

Chosen option: "[Patrón Mediator] ", because [necesitamos un canal de mensajeria mediante el cual los microservicios se comuniquen independientemente y de forma asincrona. El patrón Mediator nos proporciona la posibilidad de hacer esto.].

### Positive Consequences 

* [La comunicación entre objetos es encapsulada con un objeto mediador.]
* [Los objetos no se comunican de forma directa entre ellos, en lugar de ello se comunican mediante el mediador.]
* [Reduce las dependencias entre los objetos en comunicación.]

### Negative Consequences 

* [Hay que crear un objeto mediador.]

## Links

* [ADD-20](https://github.com/CarlotaMenendez/PracticaDAS/blob/main/docs/adr/ADD-20-Patrón-Bus.md) [ADD-20-Patrón-Bus.md]

<!-- markdownlint-disable-file MD013 -->
