# Software Requirements Specification

## For DueTo
## Version 1.0

## Revision History

|**Date**|**Version**|**Description**|**Author**|
| :-: | :-: | :-: | :-: |
|22/10/21|1.0|\<details\>|DueTo-Team|
| | | | |
| | | | |
| | | | |

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

        -   [2.3 User characteristics](#23-user-characteristics)
        -   [2.4 Dependencies](#24-dependencies)

    -   [3. Specific Requirements](#3-specific-requirements)

        -   [3.1 Functionality – Data Backend](#31-functionality--data-backend)

            -   [3.1.1 Read data given over API endpoints](#311-read-data-given-over-api-endpoints)
            -   [3.1.2 Parse data](#312-parse-data)
            -   [3.1.3 Provide data](#313-provide-data)

        -   [3.2 Functionality – User Interface](#32-functionality--user-interface)

            -   [3.2.1 User system](#321-user-system)

        -   [3.3 Usability](#33-usability)

        -   [3.4 Reliability](#34-reliability)

            -   [3.4.1 Availability](#341-availability)
            -   [3.4.2 MTBF, MTTR](#342-mtbf-mttr)
            -   [3.4.3 Accuracy](#343-accuracy)
            -   [3.4.4 Bug classes](#344-bug-classes)

        -   [3.5 Performance](#35-performance)

            -   [3.5.1 Response time](#351-response-time)
            -   [3.5.2 Throughput](#352-throughput)
            -   [3.5.3 Capacity](#353-capacity)
            -   [3.5.4 Resource utilization](#354-resource-utilization)

        -   [3.6 Supportability](#36-supportability)

        -   [3.7 Design Constraints](#37-design-constraints)

            -   [3.7.1 Development tools](#371-development-tools)
            -   [3.7.2 Spring Boot](#372-spring-boot)
            -   [3.7.3 ReactJS](#373-reactjs)
            -   [3.7.4 Supported Platforms](#374-supported-platforms)

        -   [3.8 Online User Documentation and Help System Requirements](#38-online-user-documentation-and-help-system-requirements)

        -   [3.9 Purchased Components](#39-purchased-components)

        -   [3.10 Interfaces](#310-interfaces)

            -   [3.10.1 User Interfaces](#3101-user-interfaces)
            -   [3.10.2 Hardware Interfaces](#3102-hardware-interfaces)
            -   [3.10.3 Software Interfaces](#3103-software-interfaces)
            -   [3.10.4 Communications Interfaces](#3104-communications-interfaces)

        -   [3.11 Licensing Requirements](#311-licensing-requirements)

        -   [3.12 Legal, Copyright and other Notices](#312-legal-copyright-and-other-notices)

        -   [3.13 Applicable Standards](#313-applicable-standards)

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

### 2.3 User characteristics

Our usergroup spans across ages and jobs. Everybody who lents money to someone and the other way round is part of our targeted usergroup.

### 2.4 Dependencies

to be determined (tbd)

## 3. Specific Requirements

### 3.1 Functionality – Data Backend

to be determined (tbd)

#### 3.1.1 Read data given over API endpoints

to be determined (tbd)

#### 3.1.2 Parse data

to be determined (tbd)

#### 3.1.3 Provide data

to be determined (tbd)

### 3.2 Functionality – User Interface

The frontend provides an user interface for the users to interact with and is able to request data from the data backend. The following subsections explain the types of data the frontend can request.
According uses cases are:

-   [FAQ](https://)

#### 3.2.1 User system

...
According use cases are:

-   [to be determined (tbd)](https://)




### 3.3 Usability

to be determined (tbd)

### 3.4 Reliability

to be determined (tbd)

#### 3.4.1 Availability

to be determined (tbd)

#### 3.4.2 MTBF, MTTR

to be determined (tbd)

#### 3.4.3 Accuracy

to be determined (tbd)

#### 3.4.4 Bug classes

We classify bugs like the following:

-   **Critical bug**: A critical bug occurs when the database starts dropping data without intention, secret user information, like passwords, are open to the public or users are not able to use the application at all.
-   **Non critical bug**: A non critical bug appears when the user still can use the application but it appears glitched and the user experience is slightly influenced.

### 3.5 Performance

to be determined (tbd)

#### 3.5.1 Response time

to be determined (tbd)

#### 3.5.2 Throughput

to be determined (tbd)

#### 3.5.3 Capacity

to be determined (tbd)

#### 3.5.4 Resource utilization

to be determined (tbd)

### 3.6 Supportability

to be determined (tbd)

### 3.7 Design Constraints


#### 3.7.1 Development tools

-   Git: version control system
-   JetBrains IntelliJ: Spring MVC backend development
-   Visual Studio Code: React JS frontend development
-   Maven: Backend Build management
-   NPM: Frontend Build management
-   Jira: Project planning tool
-   Github Actions: Continous integration service

#### 3.7.2 Spring Boot

to be determined (tbd)

#### 3.7.3 ReactJS

to be determined (tbd)

#### 3.7.4 Supported Platforms

to be determined (tbd)

### 3.8 Online User Documentation and Help System Requirements

to be determined (tbd)

### 3.9 Purchased Components

-   to be determined (tbd)

### 3.10 Interfaces

#### 3.10.1 User Interfaces

to be determined (tbd)

#### 3.10.2 Hardware Interfaces

-   to be determined (tbd)

#### 3.10.3 Software Interfaces

-   to be determined (tbd)

#### 3.10.4 Communications Interfaces

to be determined (tbd)

### 3.11 Licensing Requirements

to be determined (tbd)

### 3.12 Legal, Copyright and other Notices

-   to be determined (tbd)

### 3.13 Applicable Standards

-   to be determined (tbd)

## 4. Supporting Information

For a better overview, watch the table of contents and/or references.
