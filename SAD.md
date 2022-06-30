# Software Architecture Document

## Table of Contents

-   [Software Architecture Document](#software-architecture-document)

-   [Table of Contents](#table-of-contents)

    -   [1. Introduction](#1-introduction)

        -   [1.1 Purpose](#11-purpose)
        -   [1.2 Scope](#12-scope)
        -   [1.3 Definitions, Acronyms and Abbreviations](#13-definitions-acronyms-and-abbreviations)
        -   [1.4 References](#14-references)
        -   [1.5 Overview](#15-overview)

    -   [2. Architectural Representation and Patterns](#2-architectural-representation)

    -   [2.1 Technologies used](#21-technologies-used)

        -   [Spring Boot (Backend)](#spring-boot-backend)
        -   [ReactJS (Frontend)](#reactjs-frontend)

    -   [3. Architectural Goals and Constraints](#3-architectural-goals-and-constraints)

    -   [4. Use-Case View](#4-use-case-view)

    -   [5. Logical View](#5-logical-view)

        -   [5.1 MVC high level diagram](#51-mvc-high-level-diagram)

        -   [5.2 Marked MVC class diagram](#52-marked-mvc-class-diagram)

    -   [6. Deployment View](#6-deployment-view)

    -   [6.1 Deployment Process](#61-deployment-process)

    -   [6.2 Deployment View](#62-deployment-view)

    -   [7. Implementation View](#7-implementation-view)

    -   [8. Data View](#8-data-view)

    -   [9. Size and Performance](#9-size-and-performance)

    -   [10. Quality/Metrics](#10-qualitymetrics)

## 1. Introduction

### 1.1 Purpose

This document provides a comprehensive architectural overview of the system, using a number of different architectural views to depict different aspects of the system. It is intended to capture and convey the significant architectural decisions which have been made on the system.

### 1.2 Scope

The scope of this SAD is to show the architecture of our DueTo project. Illustrated are the Use-Cases, the class and data structure.

### 1.3 Definitions, Acronyms and Abbreviations

| Abbrevation | Description                         |
| ----------- | ----------------------------------- |
| SRS         | Software Requirements Specification |
| UC          | Use Case                            |
| MVC         | Model View Controler                |

### 1.4 References

| Title                                                                                                                |    Date    | Publishing organization                    |
| -------------------------------------------------------------------------------------------------------------------- | :--------: | ------------------------------------------ |
| [DueTo Blog](https://sedueto.wordpress.com/)                                                 | 2021-12-07 | DueTo-Team                    |
| [Repository on GitHub](https://github.com/SE-DueTo/)                                                       | 2021-12-07 | DueTo-Team                    |
| [SRS](./SRS.md)                                                                                                      | 2021-12-07 | DueTo-Team                    |

### 1.5 Overview

This document contains the Architectural Representation, Goals and Constraints as well as the Logical, Deployment, Implementation and Data Views.

## 2. Architectural Representation and Patterns

We are trying to implement according to the MVC pattern:

![MVC structure](img/mvc_structure.png)

## 2.1 Technologies used

tl;dr; Blogpost [here!](https://sedueto.wordpress.com/2021/10/12/week-1-2-technologies-and-roles/)

IDEs:

-   Frontend: Visual Studio Code
-   Backend: IntelliJ IDEA Ultimate 

Languages:

-   Frontend: JavaScript, TypeScript HTML, CSS, JSON for data transfer
-   Backend: Java, hardly any SQL

Frameworks:

-   Frontend: ReactJS, MaterialUI
-   Backend: Spring boot, Docker

Testing (part of CI / CD Maven pipeline):

-   Frontend: Selenium for running UI tests based on Gherkin / Cucumber .feature files
-   Backend: JUnit 5

Metrics & Patterns (part of CI / CD Maven pipeline):

-  [Metrics](https://sedueto.wordpress.com/2022/06/03/2-8-metrics/):
 [SonarCloud](https://sonarcloud.io/organizations/se-dueto/projects), 
[Codacy Backend](https://app.codacy.com/gh/SE-DueTo/DueTo-Backend/dashboard),
[Codacy Frontend](https://app.codacy.com/gh/SE-DueTo/dueto-frontend/dashboard?branch=main) 

- [Patterns](https://sedueto.wordpress.com/2022/05/20/week-2-7-design-patterns/)

Deployment (part of CI / CD mentioned Travis pipeline):

-   Docker
-   Apache2

In detail:

### Spring Boot (Backend)

Spring Boot is built on top of the Java Spring framework and provides the developer with helpful features to create and run web applications. In our case, a REST Web Service
which represents the interface between our front- and backend. As we want to benefit from the newest features of Java 10, the platform this service will be hosted on needs to support Java 10 or higher.

We use InteliJ IDEA Ultimate for coding in the backend. The backend will be written with pure Java. Only to fill our database with testable content we use one file SQL.

### ReactJS (Frontend)

ReactJS helps building interactive UIs that can be updated dynamically and therefore eliminate the need to refresh the web application. One can also develop single
components and can reuse them all over the application. Such a component could be a login form, a profile card or anything else one wants to reuse. We are going to
import a React framework called Material-UI that provides a lot of pre-defined components. Its design based on the Material-Design of Google. The development will
take place with the newest version of JavaScript. Fortunately, our development environment is able to compile it to the lower version of JavaScript. Thus, we can
use the newest features without having to worry about browser compatibility.

We use Visual Studio Code for coding in the frontend. To display we use HTML and CSS and for functionality we use JavaScript.

## 3. Architectural Goals and Constraints

We decided to use Spring MVC as our main framework. It allows us to unite backend, frontend development and the database integration in one code base. The backend runs a MySQL data base in a Docker container. Docker works great in packaging an application or a software into one single "unit", which you can then deploy anywhere as long as Docker engine is installed. It expects the package, or image to be run as a single process per container. With Docker a MySQL image is build, using a specific version and vendor, the image is packaged and distributed to anybody who wants to quickly fire a MySQL instance.

## 4. Use-Case View

Our Use-Case-Diagram

![UseCaseDiagram](https://drive.google.com/uc?id=1cm9gGoyGPQBgYl-CeENYOEPFsI-1e7nx)

## 5. Logical View

### 5.1 MVC high level diagram
![MVC high level diagram](img/mvc_structure.png)

### 5.2 Marked MVC class diagram

![MVC marked diagram](img/mvc_architecture.png)

## 6. Deployment View

### 6.1 Deployment Process

![Deployment View](https://drive.google.com/uc?id=1ONnJIUAL-fyRoChHP6SaufGdWcy37V09)

Because Google Drive is weird: [Link](https://drive.google.com/file/d/1ONnJIUAL-fyRoChHP6SaufGdWcy37V09/view?usp=sharing)

### 6.2 Deployment View

Our Service are hosted on a DHBW-Server, running a Apache2 Server to relay requests to our static frontend, or to proxy these requests into a virtual network, running our Backend and database.

Hardware (a bit overpowered :) ):
- 2 CPU cores
- 4 GB RAM
- 40 GB storage


## 7. Implementation View

-   n/a

## 8. Data View

The following graphic describes the relationship model of the in use data base

Relationship Model
![Relationship Model](https://drive.google.com/uc?id=1nHTh1wwdvAp0_Q6aGNdHvT5h5j7aE481)

Real world Model
![Real world Model](img/er_diagram.png)

Class Diagram
![Class Diagram](https://github.com/SE-DueTo/DueTo-Documentation/raw/main/img/class_diagram.png)

## 9. Size and Performance

-   n/a

## 10. Quality/Metrics

We used Codacy and SonarCloud to control our code quality, in which the Frontend and the Backend got an A. We used the integrated tools of IntelliJ to calculate our test coverage. The Unit Test as well as the API-Test are used to ensure that our application runs without any errors.

The Cyclomatic complexity is a metric we took a look at in our Backend, to ensure that all request are fast, and the program has as few as possible decisions to make.

[Metrics blog post](https://sedueto.wordpress.com/2022/06/03/2-8-metrics/):

- [SonarCloud](https://sonarcloud.io/organizations/se-dueto/projects)
- [Codacy Backend](https://app.codacy.com/gh/SE-DueTo/DueTo-Backend/dashboard)
- [Codacy Frontend](https://app.codacy.com/gh/SE-DueTo/dueto-frontend/dashboard?branch=main) 
