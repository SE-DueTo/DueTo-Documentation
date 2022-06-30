# Software Requirements Specification

## DueTo Team

## Table of Contents

-   [Flashcard Community - Software Requirements Specification](#flashcard-community---software-requirements-specification)

    -   [Table of Contents](#table-of-contents)

    -   [1. Introduction](#1-introduction)

        -   [1.1 Purpose](#11-purpose)

        -   [1.2 Scope](#12-scope)

        -   [1.3 Definitions, Acronyms and Abbreviations](#13-definitions-acronyms-and-abbreviations)
        -   [1.4 References](#14-references)
        -   [1.5 Overview](#15-overview)

    -   [2. Overall Description](#2-overall-description)

        -   [2.1 Vision](#21-vision)

        -   [2.2 Product perspective](#22-product-perspective)
        -   [2.3 Technology Stack](#23-technology-stack)

        -   [2.4 User characteristics](#24-user-characteristics)

    -   [3. Specific Requirements](#3-specific-requirements)

        -   [3.1 Functionality](#31-functionality)

        -   [3.2 Usability](#32-usability)

            -   [3.2.1 No training needed](#321-no-training-needed)

        -   [3.3 Reliability](#33-reliability)

            -   [3.3.1 Availability](#331-availability)

            -   [3.3.2 Defect Rate](#332-defect-rate)

            -   [3.3.3 Bug classes](#333-bug-classes)

        -   [3.4 Performance](#34-performance)

            -   [3.4.1 Capacity](#341-capacity)

            -   [3.4.2 Storage](#342-storage)

            -   [3.4.3 App perfomance / Response time](#343-app-perfomance-/-response-time)

        -   [3.5 Performance](#35-performance)

            -   [3.5.1 Coding Standards](#351-coding-standards)
            -   [3.5.2 Testing Strategy](#352-testing-strategy)

        -   [3.6 Design Constraints](#36-design-constraints)

            -   [3.6.1 Development tools](#361-development-tools)

            -   [3.6.2 Supported Platforms](#362-supported-platforms)

        -   [3.7 Interfaces](#37-interfaces)

            -   [3.7.1 User Interfaces](#371-user-interfaces)

    -   [4. Supporting Information](#4-supporting-information)

## 1. Introduction

### 1.1 Purpose

This document gives a general description of the DueTo Project. It explains our vision and all features of the product. Also it offers insights into the system of back- and frontend, the interfaces in both ends for communication and the constraints of the product.

### 1.2 Scope

This document is designed for internal use only and will outline the development process of the project.

### 1.3 Definitions, Acronyms and Abbreviations

| Term     |                                     |
| -------- | ----------------------------------- |
| **SRS**  | Software Requirements Specification |
| **tbd**  | to be determined |
| **n/a**  | not applicable |
| **UC**  | Use Case |
| **UI**  | Use Interface |



### 1.4 References

| Title                                                                                                 | Date       |
| ----------------------------------------------------------------------------------------------------- | ---------- |
| [Blog](https://sedueto.wordpress.com/)                                                     | 17/10/2021 |
| [GitHub](https://github.com/SE-DueTo/fc-com/)                                                     | 17/10/2021 |
| [Spring Boot](https://spring.io/projects/spring-boot)                                                 | 19/10/2021 |
| [ReactJS](https://reactjs.org/)                                                                       | 19/10/2021 |
| [Use Case Diagram](https://) | 21/10/2021 |

### 1.5 Overview

The next chapters provide information about our vision based on the use case diagram as well as more detailed software requirements.

## 2. Overall Description

### 2.1 Vision

DueTo is a financial management tool for groups or individuals that helps with your dues. When lending money the tool helps you track who has to pay you how much and vice versa, everything contained in a modern looking design.

## 2.2 Product perspective

Our Use-Case-Diagram

![UseCaseDiagram](https://drive.google.com/uc?id=1cm9gGoyGPQBgYl-CeENYOEPFsI-1e7nx)

### 2.3 Technology Stack
We chose a rather typical modern Web-Tech Stack because of existing expertise in the team and relevance for the companies we work for.

Frontend

    ReactJS
    Javascript
    Typescript
    CSS
    MaterialUI

Backend

    Spring-Boot
    Docker
    MySQL

Version control

    Git
    Github (https://github.com/SE-DueTo)

Integrated development environments (IDE)

    Microsoft Visual Studio Code
    Jetbrains IntelliJ

### 2.4 User characteristics

Our user group spans across ages and jobs. Everybody who lents money to someone and the other way around is part of our targeted user group.

## 3. Specific Requirements

### 3.1 Functionality

This section contains the different use cases and their functionality. The separate use cases can be found in the links below: 

- [Add Group](https://github.com/SE-DueTo/DueTo-Documentation/blob/main/UC/UC-AddGroup.md)

- [Add Group Member](https://github.com/SE-DueTo/DueTo-Documentation/blob/main/UC/UC-AddGroupMember.md)

- [Settle Debt](https://github.com/SE-DueTo/DueTo-Documentation/blob/main/UC/UC-SettleDebt.md)

- [Show Debt](https://github.com/SE-DueTo/DueTo-Documentation/blob/main/UC/UC-showDebts.md)

- [Add Transaction](https://github.com/SE-DueTo/DueTo-Documentation/blob/main/UC/UC_AddTransaction.md)

- [CRUD Groups](https://github.com/SE-DueTo/DueTo-Documentation/blob/main/UC/CRUD_Groups.md)

- [CRUD Transaction](https://github.com/SE-DueTo/DueTo-Documentation/blob/main/UC/CRUD_Transaction.md)
### 3.2 Usabilty

The frontend provides a user interface for the users to interact with and is able to request data from the data backend. We designed the user interface as intuitive and self-explanatory as possible to make the user feel comfortable using the app. The UI is minimalistic and not crowded and overwhelming. In this way, the information the user searches for should be easily readable and the user should be able to quickly navigate through the website.

#### 3.2.1 No training needed

Our goal is that a user searches up the application, opens it and is able to use all features without any explanation or help.

### 3.3 Reliability

#### 3.3.1 Availability

The Application does not communicate with other instances of itself. Therefore, the uptime should be 99% as long as a working version of the application is available. The only thing that can fail is the data base that provides the user, group and transaction information, so that the user gets a corresponding notification.

3.3.2 Defect Rate

The goal is that there is no loss of any data within our services.

#### 3.3.3 Bug classes

We classify bugs like the following:

-   **Critical bug**: A critical bug occurs when the database starts dropping data without intention, secret user information, like passwords, are open to the public or users are not able to use the application at all.
-   **Non critical bug**: A non critical bug appears when the user still can use the application but it appears glitched and the user experience is slightly influenced.

### 3.4 Performance

#### 3.4.1 Capacity

The system should be able to manage to run on low computing power devices to make it accessible to as many people as possible.

#### 3.4.2 Storage

The backend runs a MySQL data base in a Docker container. Docker works great in packaging an application or a software into one single "unit", which you can then deploy anywhere as long as Docker engine is installed. It expects the package, or image to be run as a single process per container. With Docker a MySQL image is build, using a specific version and vendor, the image is packaged and distributed to anybody who wants to quickly fire a MySQL instance.

#### 3.4.3 App perfomance / Response time

To provide the best App perfomance we aim to keep the response time as low as possible. This will make the user experience much better.

### 3.5 Supportability

#### 3.5.1 Coding Standards

We are going to write the code by using all of the most common clean code standards, e. g. we will name our variables and methods by their functionalities. This keeps the code easy to read by everyone and make further developement much easier. We will be also using different design patterns to make modifications of the code easier in the future and also make our code more understandable. For this, we settled on using the SOFA principle, DTOs and Mappers. You can find more about this topic [here](https://sedueto.wordpress.com/2022/05/20/week-2-7-design-patterns/)
 
#### 3.5.3 Testing Strategy

 - Integrated testing (API is reachable, can connect to the data base and returns a value)
- Unit tests (Frontend, Backend)
- UI tests (Cucumber)

### 3.6 Design Constraints

We are trying to provide a modern and easy to handle design for the UI. The architecture of our app should also be kept simple. To achieve that the functionalities will be kept as modular as possible.

#### 3.6.1 Development tools

-   Git: version control system
-   JetBrains IntelliJ: Spring MVC backend development
-   Visual Studio Code: React JS frontend development
-   Maven: Backend Build management
-   NPM: Frontend Build management
-   Jira: Project planning tool
-   Github Actions: Continous integration service

Because we are progamming a website with React, we chose Typescript/JavaScript for our front end. Also we are using the basic frontend - backend principle to keep UI-referred seperated from the backend services. To make the communication between the two parts easy, we implemented a RESTful-API between them which will provide the data in JSON-Format. We also use Docker containers to run MySQL data base.

#### 3.6.2 Supported Platforms

Any internet-capable device.

### 3.7 Interfaces

#### 3.7.1 User Interfaces

The User interfaces that will be implented are:

- Login - a login page will be available
- Register - provides a registration form
- User Dashboard - lists of all debts and transactions
- User-User Dashboard - a dashboard, containg two people. It lists all debts and transactions between the two members
- Transactions - the user is able to add a transaction in order to pay the owned amount of money
- Debts - the user can see and settle the debts that he/she has

### 3.8 Legal, Copyright and other Notices

We do not take responsibilty for any incorrect data or errors in the application.
## 4. Supporting Information

For a better overview, watch the table of contents and/or references.
