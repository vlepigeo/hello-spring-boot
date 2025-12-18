# Hello Spring Boot

Projet Hello World simple avec Spring Boot.

## Prérequis

- Java 17 ou supérieur
- Maven 3.6+

## Installation

1. Cloner le repository :
```bash
git clone https://github.com/vlepigeo/hello-spring-boot.git
cd hello-spring-boot
```

2. Compiler le projet :
```bash
mvn clean install
```

## Lancer l'application

```bash
mvn spring-boot:run
```

L'application démarre sur http://localhost:8080

## Endpoints disponibles

- `GET /` - Retourne "Hello World from Spring Boot!"
- `GET /hello?name=YourName` - Retourne "Hello YourName!"

## Exemples

```bash
# Test endpoint principal
curl http://localhost:8080/

# Test avec paramètre
curl http://localhost:8080/hello?name=Claude
```

## Structure du projet

```
hello-spring-boot/
├── src/
│   └── main/
│       ├── java/
│       │   └── com/example/hello/
│       │       ├── HelloApplication.java
│       │       └── HelloController.java
│       └── resources/
│           └── application.properties
├── pom.xml
└── README.md
```