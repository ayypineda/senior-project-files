OSSA Test Plan Document
==================

- [IDENTIFICATION INFORMATION](#identification-information)
  - [Product](#product)
  - [Project Description](#project-description)
  - [Testing Objectives](#testing-objectives)
  - [Features to be Tested](#features-to-be-tested)
  - [Features Not to Be Tested](#features-not-to-be-tested)
- [UNIT TEST](#unit-test)
  - [UNIT TEST STRATEGY / EXTENT OF UNIT TESTING:](#unit-test-strategy--extent-of-unit-testing)
  - [UNIT TEST CASES](#unit-test-cases)
- [REGRESSION TEST](#regression-test)
  - [Regression Test Strategy](#regression-test-strategy)
  - [Regression Test Cases](#regression-test-cases)
- [INTEGRATION TEST](#integration-test)
  - [Integration Test Strategy and Extent of Integration Testing](#integration-test-strategy-and-extent-of-integration-testing)
  - [Integration Test Cases](#integration-test-cases)
- [USER-ACCEPTANCE TEST (To be completed by the business office)](#user-acceptance-test-to-be-completed-by-the-business-office)
  - [User-Acceptance Test Strategy](#user-acceptance-test-strategy)
  - [User-Acceptance Test Cases](#user-acceptance-test-cases)
- [Test Deliverables](#test-deliverables)
- [Schedule](#schedule)
- [Risks](#risks)
- [Appendix](#appendix)


IDENTIFICATION INFORMATION
--------------------------

### Product

- **Product Name:** Open Source Security Auditor

### Project Description

This is an open-source online security audit tool that checks popular databases for personal information, as well as forms for their respective takedown and scrubbing requests.

### Testing Objectives

The test plan is to implement the tools necessary for quick takedown and scrubbing if and when a potential security risk presents itself. The features will be tested using the user's information per unit of every phase.

### Features to be Tested

1. Fast PPI Lookup with Freeware 
2. Security Health Checklist with Best Practices
3. Takedown Requests Forms and Scrubbing Methods

### Features Not to Be Tested

(List the features of the software/product which will not be tested. Specify the
reasons these features won’t be tested.)
1. The Fast PPI Lookup will not be tested because of the difficulty at the moment with requesting data from a browser with another API.

UNIT TEST
---------

### UNIT TEST STRATEGY / EXTENT OF UNIT TESTING:

New Features:
- safety checklist
- link checker
- ppi checker 
- takedown forms with frequent updates

Test Environment:
- x64 machine with Windows 10 or later
- Google Chrome, Safari, or Mozilla at latest versions(respectively)
- 4GB RAM
- integrated graphics
- Intel i5 processor

### UNIT TEST CASES

| \#  | OBJECTIVE | INPUT | EXPECTED RESULTS | TEST DELIVERABLES |
| --: | --------- | ----- | ---------------- | ----------------- |
|  1  | PPI Lookup  |   user's name and state    |     basic ppi             |       N/A            |
|  2  |     safety checklist      |   markup of checklist    |      assurance in safety         |      the program continues to main page         |


REGRESSION TEST
---------------

Ensure that previously developed and tested software still performs after change.

### Regression Test Strategy

- Evaluate all reports introduced in previous releases.
- Isolate problematic modules
- Revert back to latest functioning version
- Optimize integration

### Regression Test Cases

| #   | OBJECTIVE | INPUT | EXPECTED RESULTS | OBSERVED |
| --: | --------- | ----- | ---------------- | -------- |
|  1  |   implement link lookup    | basic user info and domain   |  checklist, takedown section still function  |   N/A    |
|  2  |   implement safety checklist        |   user checks off lsit items    |  program continues to lookups      |  functions as expected    |


INTEGRATION TEST
----------------

Combine individual software modules and test as a group.

### Integration Test Strategy and Extent of Integration Testing

Evaluate all integrations with locally developed shared libraries, with consumed services, and other touch points.

Comply with Facebook, Whitepages, etc. and their respective APIs to create for portability across platforms.

### Integration Test Cases

| #   | OBJECTIVE | INPUT | EXPECTED RESULTS | TEST DELIVERABLES |
| --: | --------- | ----- | ---------------- | ----------------- |
|  1  |   checklist does not hinder main page launch      |    checklist is filled   |     main page is launched        |  N/A        |


USER-ACCEPTANCE TEST
--------------------

Verify that the solution works for potential user. Include the method (e.g.,
heuristic, performance measures, thinking aloud, observation, questionnaire, 
interviews, etc.), the number of participants and demographics, the consent
form, *scenarios*, scripts to read, and data collection methods.

### User-Acceptance Test Strategy

- Users will read a brief summary of the purpose of the program and a brief statement of the goal and the problems it aims to solve.
- Users will be given a scenario and access to the program with which to undertake role of the user.
- The end user will make note of what was successful and what was not.
- The user will take a brief survey about the features and the goal vs. results.
 Changes will be made and then user-acceptance will be tested again until most goals are satisfied on average.

### User-Acceptance Test Cases

| #   | TEST ITEM | EXPECTED RESULTS | ACTUAL RESULTS | DATE |
| --: | --------- | ---------------- | -------------- | ---- |
|  1  |    checklist       |        informs user/delivers best practices          |     N/A     |  N/A    |
|  2  |    link checker     |    displays user ppi or exposes security breach    |    N/A        |   N/A   |


Test Deliverables
-----------------

(List test deliverables, and links to them if available, including the following.)

-   Test Plan 
-   Test Scripts
-   Defect/Enhancement Logs
-   Test Result Reports


Schedule
--------

Fall 2024
- looking for solutions
- analyzing weaknesses in social media platforms
- researching build platforms

Spring 2025
- designing UI
- creating a mockup of program
- researching best practices
- analyzing common exploits in social media interaction

Summer 2025
- implementing functions
- researching cross-API sanitation
- refining UI for user friendliness
- testing and checking for bugs

Fall 2025
- gathering users
- conducting acceptance testing
- gathering feedback
- implementing feedback
- regression testing
- making reports 

Risks
-----

-   Potential risks are exposure to available information on the end user, as well as the ability of a bad actor to use the program for mining an individual's PPI. 
-   These risks can be addressed with takedown forms and scrubbing requests, and an acknowledgement that the user's information is already public information. 


Appendix
--------

(Include any information that is helpful to reference.)
