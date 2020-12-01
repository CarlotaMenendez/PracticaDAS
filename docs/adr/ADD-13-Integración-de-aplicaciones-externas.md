# Integrar aplicaciones externas asincronas

* Status: [accepted] 
* Deciders: [Alberto Jimenez, Manuel Martin, Javier Mendez, David Mestanza] 
* Date: [01/12/2020] 

## Context and Problem Statement

[Necesitamos que nuestra aplicación pueda  integrar aplicaciones externas de forma asíncrona para reforzar la fiabilidad de los microservicios nativos de la tienda virtual.]

## Decision Drivers 

* [driver 1: RF.-7]

## Considered Options

* [ADD-13] Patrón Federación

## Decision Outcome

Chosen option: "[Patrón Federación] ", because [ En este caso  los accesos al o del exterior a cualquiera de las aplicaciones son gestionados por el sistema. Este sistema atiende las solicitudes en nombre del solicitante y se configura para exponer sólo la
información pertinente].

### Positive Consequences 

* [Consolidador de información entre varias aplicaciones]
* [Mantiene la integridad de la información entre varios sistemas.]
* [Posibilita el intercambio de información entre los sistemas en tiempo real.]

### Negative Consequences 

* [Requiere conocimiento de problematicas y aspectos tecnicos]
* [Las implementaciones deben ser extensibles y modulares para permitir cambios futuros]

<!-- markdownlint-disable-file MD013 -->
