
# DueTo – Test plan

## Table of Contents
- [Test plan](#test-plan)
    - [1. Introduction](#1-introduction)
        - [1.1 Purpose](#11-purpose)
        - [1.2 Scope](#12-scope)
        - [1.3 Intended Audience](#13-intended-audience)
        - [1.4 Document Terminology and Acronyms](#14-document-terminology-and-acronyms)
        - [1.5  References](#15--references)
    - [2. Evaluation Mission and Test Motivation](#2-evaluation-mission-and-test-motivation)
        - [2.1 Background](#21-background)
        - [2.2 Evaluation Mission](#22-evaluation-mission)
        - [2.3 Test Motivators](#23-test-motivators)
    - [3. Target Test Items](#3-target-test-items)
    - [4. Outline of Planned Tests](#4-outline-of-planned-tests)
        - [4.1 Outline of Test Inclusions](#41-outline-of-test-inclusions)
        - [4.2 Outline of Test Exclusions](#42-outline-of-test-exclusions)
    - [5. Test Approach](#5-test-approach)
        - [5.1 Testing Techniques and Types](#51-testing-techniques-and-types)
            - [5.1.1 Unit Testing](#511-unit-testing)
            - [5.1.2 User Interface Testing](#512-user-interface-testing)
            - [5.1.3 Integration Testing (API Testing)](#513-integration-testing-api-testing)
    - [6. Deliverables](#6-deliverables)
        - [6.1 Test Evaluation Summaries](#61-test-evaluation-summaries)
        - [6.2 Reporting on Test Coverage](#62-reporting-on-test-coverage)
        - [6.3 Perceived Quality Reports](#63-perceived-quality-reports)
        - [6.4 Incident Logs and Change Requests](#64-incident-logs-and-change-requests)
        - [6.5 Smoke Test Suite and Supporting Test Scripts](#65-smoke-test-suite-and-supporting-test-scripts)
    - [7. Testing Workflow](#7-testing-workflow)
    - [8. Environmental Needs](#8-environmental-needs)
        - [8.2 Base Software Elements in the Test Environment](#82-base-software-elements-in-the-test-environment)
        - [8.3 Productivity and Support Tools](#83-productivity-and-support-tools)
    - [9. Responsibilities, Staffing, and Training Needs](#9-responsibilities-staffing-and-training-needs)
        - [9.1 People and Roles](#91-people-and-roles)

## 1. Introduction

### 1.1 Purpose

The purpose of the Iteration Test Plan is to gather all of the information necessary to plan and control the test effort for a given iteration. It describes the approach to testing the software.
This Test Plan of Dueto's project has the following objectives:

- Identifies the items that should be targeted by the tests.
- Identifies the motivation for and ideas behind the test areas to be covered.
- Outlines the testing approach that will be used.
- Identifies the required resources and provides an estimate of the test efforts.

### 1.2 Scope

This document describes the procedure and the type of testing in the DueTo project. For the DueTo project, the following types of testing are used:

- Unit tests (Frontend, Backend)
- Integration (API) tests
- UI tests (Cucumber)

### 1.3 Intended Audience

This document is mainly addressed to the team-internal units that are responsible for testing.
In addition, this document is intended to provide orientation in the development and testing process for all team members.

### 1.4 Document Terminology and Acronyms

| Abbr | Abbreviation                        |
|------|-------------------------------------|
| API  | Application Programmable Interface  |
| BE   | Backend                             |
| FE   | Frontend                            |
| IAM  | Identity- and Access-Management     |
| n/a  | not applicable                      |
| SAD  | Software Architecture Document      |
| SRS  | Software Requirements Specification |
| UI   | User Interface                      |

### 1.5  References

| Title                                                                   | Date       | Publishing organization   |
| ------------------------------------------------------------------------|:----------:| ------------------------- |
| [Blog](https://sedueto.wordpress.com/)                             | Apr. 2022  | DueTo                      |
| [GitHub Repository](https://github.com/SE-DueTo)                    | Apr. 2022  | DueTo                      |
| [SRS](https://github.com/SE-DueTo/DueTo-Documentation/blob/main/SRS.md)                                                         | Apr. 2022  | Dueto                     |
| [SAD](https://github.com/SE-DueTo/DueTo-Documentation/blob/main/SAD.md)                                                         | Apr. 2022  | DueTo                      |

## 2. Evaluation Mission and Test Motivation

### 2.1 Background

Functionality testing is an important part of the product development process. By testing in different ways and with different tools, largely any malfunction of a product can be detected and then fixed. If you do not carry out sufficient testing, the responsible parties can be subject to heavy penalties if users are harmed.
What the project is about and the scope of the project can be read here: [SRS](https://github.com/SE-DueTo/DueTo-Documentation/blob/main/SRS.md), [SAD](https://github.com/SE-DueTo/DueTo-Documentation/blob/main/SAD.md) and [Documentation](https://github.com/SE-DueTo/DueTo-Documentation)

### 2.2 Evaluation Mission

In the testing phase, it is important to find all security-related and all functionality-critical bugs and errors.
In addition, a large part of the less serious functionality bugs should be found.

### 2.3 Test Motivators

At this point in the development, testing should primarily ensure the functionality of the application and prevent undesired functionality from being retrievable or missing features.

## 3. Target Test Items

- React Frontend
- Java Spring / Maven Backend
- Integration tests

## 4. Outline of Planned Tests

### 4.1 Outline of Test Inclusions

*React Frontend*:

- UI testing of Components (view, interaction, ...)
- Unit testing
- Integration testing (BE-Calls)

*Java Spring Backend*:

- JUnit testing of functionalities
- Integration testing (DB-Calls

### 4.2 Outline of Test Exclusions

The time frame of the project does not allow to cover the following test areas:

- Stress tests
- Load/performance tests
- Security tests

## 5. Test Approach

### 5.1 Testing Techniques and Types

#### 5.1.1 Unit Testing

Unit testing ensures, that the tested sourcecode works as expected. Therefore small parts of the sourcecode are tested independently.

|                       | Description                                                         |
|-----------------------|---------------------------------------------------------------------|
|Technique Objective    | Ensure that the implemented code works as expected                  |
|Technique              | Implement test methods using Jest (Frontend)        |
|Required Tools         | React (up-to-date, needs to support Jest)  , Spring Boot that supports JUnit testing        |
|Success Criteria       | All tests pass.   |
|Special Considerations | -                                                                    |


#### 5.1.2 User Interface Testing

By UI testing the application is tested from the perspective of the user. The goal of UI testing is to ensure that the UI behaves as expected.

|                       | Description                                                          |
|-----------------------|----------------------------------------------------------------------|
|Technique Objective    | Ensure that user interactions with frontend and the view work properly     |
|Technique              | Converting Cucumber .feature-files (see [feature-files](https://github.com/SE-DueTo/dueto-frontend/tree/main/features)) into UI tests with React |
|Required Tools         | Since UI tests are included in the unit tests with React, the same applies as in [5.1.1](#511-user-interface-testing) |
|Success Criteria 	|All UI tests pass. Pipeline is able to test FE
|Special Considerations | -                                                                    |

#### 5.1.3 Integration Testing (API Testing)

Api Testing is part of integration testing. Integration tests test multiple modules of an application together. The main goal of Api testing is to ensure, that the provided APIs of the Backend behave as expected.

|                       | Description                                                          |
|-----------------------|----------------------------------------------------------------------|
|Technique Objective    | Test the provided APIs with Postman       |
|Technique              | Pending decision of tool                                             |
|Required Tools         |  Postman                                                       |
|Success Criteria       | All tests pass. Pipeline is able to test BE    |
|Special Considerations | -                                                                    |


## 6. Deliverables

## 6.1 Test Evaluation Summaries

The tests in frontend and backend produce evaluation summaries. Thus, each time a pipeline is deployed, these status documents are created.

## 6.2 Reporting on Test Coverage

We used Codacy and SonarCloud to control our code quality, in which the Frontend and the Backend got an A. We used the integrated tools of IntelliJ to calculate our test coverage. The Unit Test as well as the API-Test are used to ensure that our application runs without any errors.

The Cyclomatic complexity is a metric we took a look at in our Backend, to ensure that all request are fast, and the program has as few as possible decisions to make.

[Metrics blog post](https://sedueto.wordpress.com/2022/06/03/2-8-metrics/)

- [SonarCloud test coverage](https://sonarcloud.io/organizations/se-dueto/projects)
- [Codacy Backend test coverage](https://app.codacy.com/gh/SE-DueTo/DueTo-Backend/dashboard)
- [Codacy Frontend test coverage](https://app.codacy.com/gh/SE-DueTo/dueto-frontend/dashboard?branch=main) 


## 6.3 Perceived Quality Reports

The code quality tools are SonarCloud and Codacy.

## 6.4 Incident Logs and Change Requests

The DueTo project uses an agile process model and therefore keeps a [Jira-Board](https://se2021-mmej.atlassian.net/jira/software/projects/MMEJ/boards/1) on which the tasks of a sprint can be seen and the pull-requests in github for the tasks.
The actual code can be found in [GitHub](https://github.com/SE-DueTo).

## 7. Testing Workflow

1) Local testing in the IDE
2) Commit and Push triggers build and test in the Code Pipeline
3) Before the automated deployment the build and test stages are executed

## 8. Environmental Needs

### 8.1 Base Software Elements in the Test Environment

The following base software elements are required in the test environment for this Test Plan.

| Software Element Name |  Type and Other Notes                        |
|-----------------------|----------------------------------------------|
| IDE                   | IntelliJ and Visual Studio Code                        |              |
| JUnit                 | Unit testing library                         |
| Cucumber              | human readable test definitions              |

### 8.2 Productivity and Support Tools

The following tools will be employed to support the test process for this Test Plan.

| Tool Category or Type | Tool Brand Name                              |
|-----------------------|----------------------------------------------|
| Repository            | [github.com](https://github.com/SE-DueTo)|
| Test Coverage FE | [SonarCloud](https://sonarcloud.io/organizations/se-dueto/projects),  [Codacy Frontend](https://app.codacy.com/gh/SE-DueTo/dueto-frontend/dashboard?branch=main) |
| Test Coverage BE | [SonarCloud](https://sonarcloud.io/organizations/se-dueto/projects), [Codacy Backend](https://app.codacy.com/gh/SE-DueTo/DueTo-Backend/dashboard) |

## 9. Responsibilities, Staffing, and Training Needs

### 9.1 People and Roles

| Role          | Person Assigned | Specific Responsibilities or Comments |
|---------------|:---------------:|---------------------------------------|
| Test Manager  | whole team         | Provides management oversight.        |
| Test Designer | whole team      | Defines the technical approach to the implementation of the test effort. |
| Test System Administrator | whole team | Ensures test environment and assets are managed and maintained. |


## 10. Risks, Dependencies, Assumptions, and Constraints

| Risk | Mitigation Strategy | Contingency (Risk is realized) |
|------|---------------------|--------------------------------|
| Too much focus on tests and too little on functions | Test only important and complex functions | write clean code |
| False certainty through false tests | The one who writes the functionality should also write the tests | take your time |
| Different interpretations of a functionality | write tests first | Delimit functionality unambiguously through tests |

## 11. Management Process and Procedures

n/a