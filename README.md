
# Teoría y Conceptos Fundamentales de GraphQL con Spring

## Tabla de Contenido

- [Introducción a GraphQL](#introduccion-graphql)
  - [¿Qué es GraphQL?](#que-es-graphql)
  - [Principios Fundamentales](#principios-fundamentales)
  - [El Problema del Over-fetching y Under-fetching](#problema-fetching)
  - [GraphQL vs. REST (Comparación Detallada)](#graphql-vs-rest)

- [El Lenguaje de Esquema (Schema Definition Language)](#lenguaje-esquema)
  - [El Sistema de Tipos](#sistema-tipos)
    - [Tipos de Objeto (Object Types)](#object-types)
    - [Tipos Escalares (Scalar Types)](#scalar-types)
    - [Tipos de Entrada (Input Types)](#input-types)
    - [Interfaces y Unions](#interfaces-unions)
    - [Enums](#enums)
  - [Definición de Esquema (`schema`)](#definicion-esquema)
  - [La Raíz del Esquema: `Query`, `Mutation` y `Subscription`](#raiz-esquema)

- [Queries y Mutaciones](#queries-mutaciones)
  - [Estructura de una Query](#estructura-query)
    - [Campos y Argumentos](#campos-argumentos)
    - [Alias, Fragmentos y Variables](#alias-fragmentos-variables)
  - [Mutation: Modificando Datos](#mutation-datos)
    - [Definición de Mutations en el Esquema](#mutations-esquema)
    - [El Flujo de una Mutation](#flujo-mutation)
  - [Resolvers](#resolvers)
    - [El Rol de los Resolvers](#rol-resolvers)
    - [Resolvers de Relaciones](#resolvers-relaciones)
    - [Resolución de Campos Nulos](#campos-nulos)

- [Suscripciones (Subscriptions)](#suscripciones)
  - [Concepto y Flujo de Datos](#concepto-flujo)
  - [Diferencias con Queries y Mutations](#diferencias-suscripciones)
  - [Implementación con WebSockets](#implementacion-websockets)
  - [Manejo del Estado de la Conexión](#estado-conexion)

- [Manejo de Errores y Validación](#errores-validacion)
  - [Errores a Nivel de GraphQL](#errores-graphql)
  - [Validación de Entrada en el Resolutor](#validacion-entrada)
  - [Mejores Prácticas de Reporte de Errores](#mejores-practicas-errores)

- [Clientes GraphQL](#clientes-graphql)
  - [Conceptos del Cliente](#conceptos-cliente)
    - [Caching](#caching)
    - [Normalización de Datos](#normalizacion-datos)
  - [Herramientas y Librerías (ej. Apollo Client)](#herramientas-librerias)

- [Integración con Spring Boot](#integracion-spring-boot)
  - [Dependencias y Configuración](#dependencias-configuracion)
  - [Escribiendo Resolvers con Spring](#escribiendo-resolvers)
    - [`@QueryMapping`](#querymapping)
    - [`@MutationMapping`](#mutationmapping)
    - [`@SubscriptionMapping`](#subscriptionmapping)
    - [Mapeo de Argumentos y Contexto](#mapeo-argumentos)
  - [Manejo de Transacciones y Persistencia](#transacciones-persistencia)
  - [Test de Integración para Endpoints GraphQL](#test-integracion)


<a id="introduccion-graphql"></a>
## Introducción a GraphQL

<a id="que-es-graphql"></a>
### ¿Qué es GraphQL?

<a id="principios-fundamentales"></a>
### Principios Fundamentales

<a id="problema-fetching"></a>
### El Problema del Over-fetching y Under-fetching

<a id="graphql-vs-rest"></a>
### GraphQL vs. REST (Comparación Detallada)


<a id="lenguaje-esquema"></a>
## El Lenguaje de Esquema (Schema Definition Language)

<a id="sistema-tipos"></a>
### El Sistema de Tipos

<a id="object-types"></a>
#### Tipos de Objeto (Object Types)

<a id="scalar-types"></a>
#### Tipos Escalares (Scalar Types)

<a id="input-types"></a>
#### Tipos de Entrada (Input Types)

<a id="interfaces-unions"></a>
#### Interfaces y Unions

<a id="enums"></a>
#### Enums

<a id="definicion-esquema"></a>
### Definición de Esquema (`schema`)

<a id="raiz-esquema"></a>
### La Raíz del Esquema: `Query`, `Mutation` y `Subscription`


<a id="queries-mutaciones"></a>
## Queries y Mutaciones

<a id="estructura-query"></a>
### Estructura de una Query

<a id="campos-argumentos"></a>
#### Campos y Argumentos

<a id="alias-fragmentos-variables"></a>
#### Alias, Fragmentos y Variables

<a id="mutation-datos"></a>
### Mutation: Modificando Datos

<a id="mutations-esquema"></a>
#### Definición de Mutations en el Esquema

<a id="flujo-mutation"></a>
#### El Flujo de una Mutation

<a id="resolvers"></a>
### Resolvers

<a id="rol-resolvers"></a>
#### El Rol de los Resolvers

<a id="resolvers-relaciones"></a>
#### Resolvers de Relaciones

<a id="campos-nulos"></a>
#### Resolución de Campos Nulos


<a id="suscripciones"></a>
## Suscripciones (Subscriptions)

<a id="concepto-flujo"></a>
### Concepto y Flujo de Datos

<a id="diferencias-suscripciones"></a>
### Diferencias con Queries y Mutations

<a id="implementacion-websockets"></a>
### Implementación con WebSockets

<a id="estado-conexion"></a>
### Manejo del Estado de la Conexión


<a id="errores-validacion"></a>
## Manejo de Errores y Validación

<a id="errores-graphql"></a>
### Errores a Nivel de GraphQL

<a id="validacion-entrada"></a>
### Validación de Entrada en el Resolutor

<a id="mejores-practicas-errores"></a>
### Mejores Prácticas de Reporte de Errores

<a id="clientes-graphql"></a>
## Clientes GraphQL

<a id="conceptos-cliente"></a>
### Conceptos del Cliente

<a id="caching"></a>
#### Caching

<a id="normalizacion-datos"></a>
#### Normalización de Datos

<a id="herramientas-librerias"></a>
### Herramientas y Librerías (ej. Apollo Client)


<a id="integracion-spring-boot"></a>
## Integración con Spring Boot

<a id="dependencias-configuracion"></a>
### Dependencias y Configuración

<a id="escribiendo-resolvers"></a>
### Escribiendo Resolvers con Spring

<a id="querymapping"></a>
#### `@QueryMapping`

<a id="mutationmapping"></a>
#### `@MutationMapping`

<a id="subscriptionmapping"></a>
#### `@SubscriptionMapping`

<a id="mapeo-argumentos"></a>
#### Mapeo de Argumentos y Contexto

<a id="transacciones-persistencia"></a>
### Manejo de Transacciones y Persistencia

<a id="test-integracion"></a>
### Test de Integración para Endpoints GraphQL
