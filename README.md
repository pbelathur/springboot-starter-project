# Spring Boot Starter Project

### Purpose
A _ready to use_ web application based on Spring Boot v2.2.4.  
This application contains the following:
* Spring Boot actuator, devtools and web starters.
* Lombok dependency and annotation processing.
* Actuator endpoints for info, health and metrics.
* Enabled junit5 and explicit exclusion of junit4.
* DB2, Oracle and H2 database driver dependencies
* Inclusion of GIT properties in actuator _info_ endpoint 

# Getting Started
1. Clone this repo from the Github repo
2. Open a command window in the project directory and execute `./gradlew build bootRun`
3. Verify the application is up and running `http://localhost:8080/actuator/health`

# NOTES
1. The _application version_ is set _before_ a release by updating the `version` in `gradle.properties`
   this should be done automatically by CI/CD and **not** by developers.
2. Build instructions:
   ```
   ./gradlew clean bootJar
   java -jar ./build/libs/springboot-starter-0.0.1-SNAPSHOT.jar
   
   ```