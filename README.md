# Aplicación de Spring Boot con Arquitectura Hexagonal

Esta es una aplicación de ejemplo desarrollada en Spring Boot que sigue la arquitectura hexagonal (también conocida como arquitectura de puertos y adaptadores). La arquitectura hexagonal es una forma de estructurar una aplicación que promueve la separación de las preocupaciones y facilita la prueba y la expansión.

## Descripción de la Arquitectura

La arquitectura hexagonal se basa en el principio de que una aplicación debe estar dividida en tres capas principales:

1. **Capa de Dominio:** En esta capa, definimos las reglas de negocio y los objetos del dominio. Aquí se encuentran las entidades, los servicios y los repositorios que encapsulan la lógica del negocio.

2. **Capa de Aplicación:** Esta capa actúa como un puente entre la capa de dominio y las interfaces de entrada/salida. Contiene casos de uso o servicios de aplicación que orquestan las operaciones del dominio.

3. **Capa de Adaptadores:** Aquí se encuentran las interfaces de entrada y salida. Los adaptadores son responsables de conectar la aplicación con el mundo exterior. Pueden ser controladores REST, servicios web, adaptadores de bases de datos, etc.

## Requisitos

Asegúrate de tener instalado lo siguiente antes de ejecutar la aplicación:

- Java Development Kit (JDK) 11 o superior
- Apache Maven
- Un IDE de tu elección (por ejemplo, IntelliJ IDEA, Eclipse)

## Cómo Ejecutar la Aplicación

1. Clona este repositorio en tu máquina local:

git clone https://github.com/JordyV3/hexagonal-crud-app


2. Abre el proyecto en tu IDE.

3. Ejecuta la clase principal `Application.java` para iniciar la aplicación Spring Boot.

4. La aplicación se ejecutará en `http://localhost:8080`. Puedes acceder a los endpoints REST y probar la funcionalidad.

## Estructura del Proyecto

La estructura del proyecto se organiza de la siguiente manera:

- `src/main/java/com/app/apirest`: Contiene el código fuente de la aplicación.
- `domain`: Contiene las clases de dominio, como entidades y servicios.
- `application`: Contiene los casos de uso y servicios de aplicación.
- `adapter`: Contiene los adaptadores de entrada/salida (por ejemplo, controladores REST).
- `src/test/java/com/app/apirest`: Contiene pruebas unitarias y de integración.

## Contribuir

Si deseas contribuir a este proyecto, ¡te damos la bienvenida! Puedes hacerlo mediante pull requests y reportando problemas a través de las issues.

## Licencia

Este proyecto se distribuye bajo la licencia MIT. Consulta el archivo LICENSE para obtener más detalles.

## Contacto

Para preguntas o comentarios, no dudes en ponerte en contacto con el equipo de desarrollo:

- Nombre: Jordy Vega
- Correo electrónico: jordyvega15@email.com

¡Gracias por utilizar nuestra aplicación!
