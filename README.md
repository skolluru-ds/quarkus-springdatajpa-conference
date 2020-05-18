
# Setup GitHub Repository
### Create new github repository
    - Copy the github project path
### Create a new project file directory on your local machine
    - mkdir <ProjectDirectory>
### Run 'git clone' command 
    - cd <ProjectDirectory>
    - git clone <GitHubRepoPath>
# Generating quarkus project
### Create the startup project from quarkus.io
    - Select maven project
    - OPTIONAL - Use github repository name as the ArtifactId
    - Select the following quarkus extensions
        - spring-data-jpa
        - resteasy-jsonb
        - quarkus-jdbc-postgresql
### Download the zip file and extract
    - Copy the extracted files into the <ProjectDirectory> created before
### Open the project in the IDE

-----------------------------------------------
-----------------------------------------------


# quarkus-springdatajpa-conference project

This project uses Quarkus, the Supersonic Subatomic Java Framework.

If you want to learn more about Quarkus, please visit its website: https://quarkus.io/ .

## Running the application in dev mode

You can run your application in dev mode that enables live coding using:
```
./mvnw quarkus:dev
```

## Packaging and running the application

The application can be packaged using `./mvnw package`.
It produces the `quarkus-springdatajpa-conference-1.0.0-SNAPSHOT-runner.jar` file in the `/target` directory.
Be aware that it’s not an _über-jar_ as the dependencies are copied into the `target/lib` directory.

The application is now runnable using `java -jar target/quarkus-springdatajpa-conference-1.0.0-SNAPSHOT-runner.jar`.

## Creating a native executable

You can create a native executable using: `./mvnw package -Pnative`.

Or, if you don't have GraalVM installed, you can run the native executable build in a container using: `./mvnw package -Pnative -Dquarkus.native.container-build=true`.

You can then execute your native executable with: `./target/quarkus-springdatajpa-conference-1.0.0-SNAPSHOT-runner`

If you want to learn more about building native executables, please consult https://quarkus.io/guides/building-native-image.