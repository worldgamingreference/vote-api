# worldgamingreference-vote api
![Version](https://img.shields.io/badge/version-0.0.1-blue.svg?cacheSeconds=2592000)

> Manage player's vote

## Install

```sh
./mvnw mvn install
```

## Run application in dev mode

```sh
./mvnw compile quarkus:dev
```

## Run tests

```sh
./mvnw test
```

## Packaging and running the application

### Without compiled dependencies

```shell script
./mvnw package
```

It produces the `code-with-quarkus-1.0.0-SNAPSHOT-runner.jar` file in the `/target` directory and dependencies are copied into the `target/lib` directory.

### With compiled dependencies (fat-jar or über-jar)

```shell script
./mvnw package -Dquarkus.package.type=uber-jar
```

The application is runnable using `java -jar target/code-with-quarkus-1.0.0-SNAPSHOT-runner.jar`.

## Creating a native executable

### With graalvm installed

```shell script
./mvnw package -Pnative
```
### Without graalvm installed

```shell script
./mvnw package -Pnative -Dquarkus.native.container-build=true
```