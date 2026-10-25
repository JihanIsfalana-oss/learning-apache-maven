# **DOCUMENTATION OF LEARNING APACHE-MAVEN**

## Identity Author
| Name | Email | GitHub |
|------|-------|--------|
|Mochammad Jihan Isfalana| wallbreker22@gmail.com| https://github.com/JihanIsfalana-oss|

## About Apache Maven
Apache Maven is a build automation tool used primarily for Java projects. It simplifies the build process by providing a uniform build system, dependency management, and project structure. Maven uses an XML file called `pom.xml` to manage project configuration, dependencies, and plugins.

## Features of Apache Maven
- **Dependency Management**: Maven automatically downloads and manages project dependencies from a central repository, making it easier to handle libraries and frameworks.
- **Build Lifecycle**: Maven defines a standard build lifecycle with predefined phases, allowing developers to easily compile, test, package, and deploy their applications.
- **Project Structure**: Maven enforces a standard directory layout for projects, promoting consistency and best practices.
- **Plugins**: Maven supports a wide range of plugins that extend its functionality, enabling tasks such as code generation, testing, and deployment.

### Lifecycle Phases
- **mvn clean:** Cleans the project by removing the target directory and any generated files.
- **mvn compile:** Compiles the source code of the project.
- **mvn test:** Runs the unit tests of the project.
- **mvn package:** Packages the compiled code into a distributable format, such as a JAR or WAR file.
- **mvn install:** Installs the packaged code into the local Maven repository for use as a dependency in other projects.
- **mvn deploy:** Deploys the packaged code to a remote repository for sharing with other developers or teams.
- **mvn site:** Generates project documentation based on the information in the `pom.xml` file.
- **mvn validate:** Validates the project structure and configuration.
- **mvn verify:** Runs any checks to verify the project is valid and meets quality standards.
- **mvn dependency:** Displays the project's dependencies and their versions.
- **mvn help:** Provides help and information about Maven commands and plugins.
- **mvn archetype:** Generates a new project based on a predefined template or archetype.
- **mvn release:** Prepares and performs a release of the project, including versioning and tagging in the version control system.

## Getting Started with Apache Maven
### Prerequisites
- **Java Development Kit (JDK)**: Ensure that you have JDK installed on your system. Maven requires JDK to compile and run Java applications.
- **Maven Installation**: Download and install Apache Maven from the official website (https://maven.apache.org/download.cgi). Follow the installation instructions for your operating system.
- **Environment Variables**: Set the `JAVA_HOME` environment variable to point to your JDK installation directory. Also, add the Maven `bin` directory to your system's `PATH` variable.
- **Verify Installation**: Open a terminal or command prompt and run the following command to verify that Maven is installed correctly:
```bash
mvn -version
```
### Creating a Maven Project
1. Open a terminal or command prompt.
2. Navigate to the directory where you want to create your Maven project.
3. Run the following command to generate a new Maven project using the default archetype:
```bash
mvn archetype:generate
```
4. Follow the prompts to specify the groupId, artifactId, version, and package for your project.

## Building and Running a Maven Project
1. Navigate to the root directory of your Maven project (where the `pom.xml` file is located).
2. To compile the project, run the following command:
```bash
mvn compile
```
3. To run the unit tests, use the following command:
```bash
mvn test
```
4. To package the project into a JAR or WAR file, run:
```bash
mvn package
```
5. To install the packaged code into your local Maven repository, use:
```bash
mvn install
```
6. To deploy the packaged code to a remote repository, run:
```bash
mvn deploy
```

## Project Structure
The standard directory layout for a Maven project is as follows:
```
|-- root-directory
    |-- src
        |-- main
            |-- java
            |-- resources
        |-- test
            |-- java
            |-- resources
    |-- target
    |-- pom.xml
```

## Conclusion
Apache Maven is a powerful build automation tool that simplifies the management of Java projects. By providing a standardized build process, dependency management, and project structure, Maven helps developers streamline their development workflow. With its extensive plugin ecosystem and support for various lifecycle phases, Maven is an essential tool for Java developers looking to build, test, and deploy their applications efficiently.

---

#### ***This Documentation is created for learning purposes by &copy; Mochammad Jihan Isfalana - 2026.***