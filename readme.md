# S4.01 - Springboot Framework

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Maven](https://img.shields.io/badge/apache_maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)
![Gradle](https://img.shields.io/badge/gradle-02303A?style=for-the-badge&logo=gradle&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=Postman&logoColor=white)
![IntelliJ](https://img.shields.io/badge/IntelliJ_IDEA-000000.svg?style=for-the-badge&logo=intellij-idea&logoColor=white)

## Summary
This exercise will introduce you to the SPRING framework.

You will start using the HTTP protocol, use Postman, and discover
how to manage dependencies with Maven and Gradle.

## 📄 LVL 1: Spring & Maven
Access the page --> https://start.spring.io/, and generate a Spring 
boot project with the following characteristics:
- **Project**: Maven
- **Language**: Java
- **Springboot**: Last stable version
- **Group**: cat.itacademy.s04.t01.n01
- **Artifact**: S04T01N01
- **Name**: S04T01N01
- **Description**: S04T01N01
- **Package name**: cat.itacademy.s04.t01.n01
- **Packagin**: Jar
- **Java**: minimum version 11
- **Dependencies**:
    - Spring Boot DevTools
    - Spring Web

Import it into IntteliJ.

In the application.properties file, set the server.port variable 
to 9000.

We will convert this application into a REST API:
Depending on the main package, create another subpackage called 
controller, and inside it, add the HelloWorldController class.

It should have two methods:
- String hello
- String hello2

These two methods will receive a String parameter called name, and 
will return the phrase:

“Hello, “ + name + “. You are running a Maven project”.

The first method will respond to a GET request, and must be 
configured to receive the parameter as a RequestParam. 
The “name” parameter will have the default value “UNKNOWN”.

It should respond to:

http://localhost:9000/HelloWorld
http://localhost:9000/HelloWorld?name=My name

The second method will respond to a GET request, and should be 
configured to receive the parameter as a PathVariable. 
The "name" parameter is optional.

It should respond to:

http://localhost:9000/HelloWorld2
http://localhost:9000/HelloWorld2/myname

## 📄 LVL 2: Spring & Gradle
Access the page --> https://start.spring.io/, and generate a Spring 
boot project with the following characteristics:
- **Project**: Gradle
- **Language**: Java
- **Springboot**: Last stable version
- **Group**: cat.itacademy.s04.t01.n01
- **Artifact**: S04T01N01
- **Name**: S04T01N01
- **Description**: S04T01N01
- **Package name**: cat.itacademy.s04.t01.n01
- **Packagin**: Jar
- **Java**: minimum version 11
- **Dependencies**:
    - Spring Boot DevTools
    - Spring Web

Import it into IntteliJ.

In the application.properties file, set the server.port variable
to 9001.

We will convert this application into a REST API:
Depending on the main package, create another subpackage called
controller, and inside it, add the HelloWorldController class.

It should have two methods:
- String hello
- String hello2

These two methods will receive a String parameter called name, and
will return the phrase:

“Hello, “ + name + “. You are running a Maven project”.

The first method will respond to a GET request, and must be
configured to receive the parameter as a RequestParam.
The “name” parameter will have the default value “UNKNOWN”.

It should respond to:

http://localhost:9000/HelloWorld
http://localhost:9000/HelloWorld?name=My name

The second method will respond to a GET request, and should be
configured to receive the parameter as a PathVariable.
The "name" parameter is optional.

It should respond to:

http://localhost:9000/HelloWorld2
http://localhost:9000/HelloWorld2/myname

## 📄 LVL 3: Postman

This is about testing the previous projects from Postman.

Run the projects created in the two previous levels from IntelliJ, 
and show the return obtained in each project, when you call some 
of the available requests, using the created environments and 
their variables.

You will have to provide two screenshots, one for the execution 
of each environment, and two files in JSON format, with the 
exported environments.

-----

## 🔧 Technologies
- **Java 24**: Core programming language
- **Maven**: Build and dependency management
- **Gradle**: Build and dependency management
- **Git/GitHub**: version control
- **Additional dependencies**:
  - Postman

### 🛠️ SCRIPTS
```bash
mvn compile          # Compile project
mvn package          # Package in .jar
mvn clean            # Clean the project
mvn spring-boot:run  # execute the app
gradle build         # Compile project
gradle assemble      # Package in .jar
gradle clean         # Clean the project
gradle bootRun       # execute the app
```

## 📚 Additional Resources
- [Badges](https://github.com/alexandresanlim/Badges4-README.md-Profile?tab=readme-ov-file#-frameworks--library-)
- [Springboot](https://spring.io/quickstart)
- [Postman](https://learning.postman.com/docs/getting-started/first-steps/sending-the-first-request/)
- [HTTP](https://www.restapitutorial.com/httpstatuscodes)

[Back to top](#top)

