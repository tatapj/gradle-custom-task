## Description

This project demonstrates the creation of a custom Gradle task using a simple Java library project. This project also demonstrates how to manage and add external libraries using Gradle dependency management, including Google Guava and JUnit.

## Objective

The objectives of this project are:

* Create a simple custom Gradle task named `greetingTask`.
* Accept a name parameter from the command line using a Gradle project property.
* Display a personalized greeting message based on the provided parameter.
* Provide a default name when no parameter is provided.
* Add and manage external libraries using Gradle dependency management.
* Use Google Guava as an implementation dependency.
* Use JUnit for testing.
* Build and manage the project using Gradle.
* Store the project in a separate GitHub repository.

## Custom `greetingTask`

The project includes a custom Gradle task named `greetingTask`. This task accepts a name parameter through a Gradle project property and displays a personalized greeting message.

The task uses the `nama` project property. If the parameter is not provided, it uses `Gradle User` as the default name.

### Run without a parameter

./gradlew :lib:greetingTask


Output:

Hello, Gradle User! Welcome to Gradle World!


### Run with a parameter

./gradlew :lib:greetingTask -Pnama=Tata

Output:

Hello, Tata! Welcome to Gradle World!



