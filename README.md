📦 Maven Actions Demo

A simple Java project that demonstrates how to:

Write a basic Java application

Add JUnit 5 tests

Build the project using Maven

Run everything automatically using GitHub Actions CI/CD

This project prints a message and includes a test to verify the output.

🚀 Project Structure

.
├── src
│   ├── main
│   │   └── java
│   │       └── com/example/App.java
│   └── test
│       └── java
│           └── com/example/AppTest.java
├── pom.xml
└── .github
    └── workflows
        └── maven.yml

📝 App.java

A simple Java class that prints:

Hello from Maven GitHub Actions Lab!

🧪 AppTest.java

A JUnit 5 test that checks whether the message returned is correct.


🧰 Build Tool: Maven


Maven is used to:

Compile Java source code

Download required libraries

Build a JAR file

Run tests with JUnit

Your pom.xml includes JUnit 5 and the Maven Surefire Plugin for running tests.


⚙️ GitHub Actions Workflow


This project includes an automated CI pipeline:

.github/workflows/maven.yml

What it does:

Checks out the code

Installs Java 17

Runs Maven build + tests

Lists the built files inside the target/ folder

So every push runs your build automatically.

▶️ Running the Project Locally

Build the project
mvn clean package

Run the JAR
java -cp target/maven-actions-demo-1.0-SNAPSHOT.jar com.example.App

Run tests only
mvn test

📂 Output

After building, you’ll find:

target/maven-actions-demo-1.0-SNAPSHOT.jar


This is your compiled Java application.

🎯 Purpose of This Project

This repository is mainly for learning and practicing:

Maven basics

Java project structure

JUnit testing

GitHub Actions CI/CD

Perfect for beginners who want to understand how everything works together.
