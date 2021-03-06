# Denarius

A WebApp mainly designed for tracking daily expenses. Based on Spring Boot, Spring Data JPA and OpenAPI.

[![Build Status Badge](https://github.com/fschrogl-fsdev/Denarius/workflows/develop/badge.svg)](https://github.com/fschrogl-fsdev/denarius/actions?query=workflow%3Adevelop)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=at.schrogl.denarius%3Adenarius-pom&metric=alert_status)](https://sonarcloud.io/dashboard?id=at.schrogl.denarius%3Adenarius-pom)

## Requirements

- Java 11+
- PostgreSQL 10.6+

## Getting started

This application is implemented using Spring Boot framework, hence it is a self-contained JAR file application. It can
be started using the Spring Boot Maven Plugin's run goal:

```bash
mvn -pl denarius-web -am spring-boot:run
```

Or by creating the application's Spring Boot JAR and starting it directly from the command line:

```bash
mvn clean install
java -jar denarius-web/target/denarius-web-X.Y.Z.jar
```

## How to develop

When developing the application make sure to activate Maven profile ``development`` and also Spring profile
``development``. The Maven profile takes care of including Spring Boots DevTools to the project's dependencies and
the Spring profiles configures the application for development purposes, i.e. using an in-memory database.

```bash
mvn -P development -pl denarius-web -am spring-boot:run --spring.profiles.active=development
```

## Miscellaneous

### Banner art

The ASCII graphic in file ``banner.txt``, which is displayed during startup of Spring Boot applications was created
using the free [Text to ASCII Art Generator](http://patorjk.com/software/taag/) from
[Patorjk.com](http://www.patorjk.com).

### Application's logo and favicon

The application's logo and favicon are made by [Freepik](https://www.flaticon.com/authors/freepik) from
[www.flaticon.com](https://www.flaticon.com).