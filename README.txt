CI/CD Pipeline for Java Application


This repository contains a Continuous Integration (CI) pipeline for building, testing, and packaging a Java application using Jenkins. The pipeline automates various stages from source code validation to packaging and is fully integrated with code quality and coverage tools.

📌 Features
Automated Java application build and test pipeline.

Integrated code quality checks using PMD.

Code coverage reports generated with JaCoCo.

Source control with Git.

Build and dependency management with Maven.

Containerization support with Docker.

Modular Jenkins jobs stored as XML configurations.

🛠 Tools & Technologies
Java – Core programming language for the application.

Git – Version control system to manage source code.

Maven – Dependency and build management tool.

Jenkins – CI/CD automation server for building and deploying.

Docker – For containerizing the Java application (optional deployment stage).

PMD – Static code analysis tool for detecting code issues.

JaCoCo – Java Code Coverage tool for test reporting.

📂 Repository Structure
Copy
Edit
mypipelinejobs/
│── javaapp_validate.xml
│── javaapp_compile.xml
│── javaapp_codereview.xml
│── javaapp_test.xml
│── javaapp_codecoverage.xml
│── javaapp_package.xml
│── ...
mypipelinejobs: Contains Jenkins job configuration XML files for each stage in the pipeline.

🔄 Pipeline Stages
Validate
Checks out the latest code from Git and validates the project structure.

Compile
Compiles the Java source code using Maven.

Code Review (PMD)
Runs PMD for static code analysis and detects coding standard violations.

Unit Testing (JUnit)
Executes unit tests to ensure the correctness of the application.

Code Coverage (JaCoCo)
Generates a code coverage report for executed tests.

Package
Packages the Java application into a JAR/WAR file.

Docker Build 
Builds a Docker image for the application.

📊 Reports & Logs
PMD Report: View under the "PMD Warnings" link in Jenkins.

JaCoCo Report: View under the "Code Coverage" link in Jenkins.

Build Logs: Available in each job’s console output.

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
