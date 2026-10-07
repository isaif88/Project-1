# OrangeHRM Manual Testing — Test Plan

## 1. Project Overview

**Project Name:** OrangeHRM Manual Testing Project  
**Application Under Test:** OrangeHRM  
**Testing Type:** Manual Software Testing  
**Testing Approach:** Requirement-oriented, risk-based manual testing

The project aims to perform structured manual testing of the OrangeHRM web application to evaluate its functionality, usability, validation, navigation, and selected security-related behaviors.

The testing process will follow:

**Test Plan → User Stories → Acceptance Criteria → Test Cases → Test Execution → Defect Reporting → Final Test Report**

---

## 2. Objective

The main objectives of this project are to:

- Validate that application features behave according to their defined Acceptance Criteria.
- Identify unexpected or incorrect system behavior.
- Design clear and reusable manual Test Cases.
- Execute Test Cases and document actual results.
- Identify, investigate, and report confirmed defects.
- Practice professional QA documentation and defect management.
- Produce a complete end-to-end manual testing project suitable for a QA portfolio.

---

## 3. Scope

The project will cover the OrangeHRM modules available in the public demo environment.

Testing coverage will be divided into three levels based on the importance and depth of testing required.

### 🔴 Core — Full Workflow Testing

These modules will receive the highest testing priority.

The goal is to perform deep testing and derive the largest practical number of User Stories, Acceptance Criteria, Test Cases, and exploratory checks.

- Login
- Dashboard
- PIM
- Leave
- Time
- Recruitment
- Admin

For Core modules, testing will focus on:

- Main functional workflows
- Positive and negative scenarios
- Input validation
- Boundary and data validation
- Navigation
- UI behavior
- Role and permission behavior where applicable
- Dependencies between related features
- Exploratory testing
- Basic security-focused checks where applicable

---

### 🟡 Secondary — Core Features

These modules will receive solid functional coverage, but with less depth than the Core modules.

- My Info
- Performance
- Claim
- Directory

Testing will focus primarily on:

- Main functionality
- Positive and negative cases
- Input validation
- Navigation
- UI behavior
- Important edge cases
- Exploratory testing where useful

---

### 🟢 Basic / Exploratory Coverage

These modules will receive basic functional and exploratory coverage.

- Maintenance
- Buzz

The objective is to understand and test the main available functionality without attempting the same depth of coverage used for Core modules.

---

## 4. Out of Scope

The following areas are outside the scope of this project:

- Source-code-level testing
- Unit testing
- Automated UI testing
- Full penetration testing
- Performance testing
- Load testing
- Stress testing
- Infrastructure/server testing
- Database-level testing unless specifically required
- Testing functionality unavailable in the public demo environment
- Verification of developer fixes
- Regression testing of new releases
- Retesting of fixed defects

> Retesting and Regression Testing are not included in the current execution because this project is focused on discovering and documenting defects in the available demo environment rather than validating developer fixes or new releases.

---

## 5. Testing Approach

Testing will follow a **requirement-oriented and risk-based approach**.

Each feature will be structured using:

**User Story → Acceptance Criteria → Test Cases → Test Execution**

Acceptance Criteria will be the primary source for defining the expected behavior of Test Cases.

### Test Case Design

Test Cases may cover:

- Positive testing
- Negative testing
- Boundary/value validation
- Input validation
- Navigation
- UI behavior
- Role/permission behavior where applicable
- Exploratory testing
- Basic security-focused checks where applicable

Testing decisions will be based on defined Acceptance Criteria and observable application behavior rather than unsupported assumptions.

When formal requirements are unavailable, assumptions will be documented explicitly.

---

## 6. Testing Types

The following testing types will be performed where applicable:

### 6.1 Functional Testing

Verify that application features perform their intended functions correctly.

### 6.2 UI Testing

Verify:

- UI elements
- Layout
- Visibility
- Labels
- Controls
- Navigation
- User interactions

### 6.3 Negative Testing

Verify that the application handles invalid inputs and invalid user actions correctly.

### 6.4 Validation Testing

Verify:

- Required fields
- Input formats
- Validation messages
- Data constraints
- Invalid values

### 6.5 Exploratory Testing

Explore the application beyond predefined Test Cases to identify unexpected behavior and potential defects.

### 6.6 Usability-Oriented Testing

Identify obvious usability problems that may negatively affect the user's interaction with the application.

### 6.7 Basic Security-Focused Testing

Perform limited black-box security-oriented checks such as:

- Authentication behavior
- Session protection
- Unauthorized access attempts
- Basic input-safety checks

This does **not** represent a full security assessment or penetration test.

---

## 7. Test Environment

### Application

**Application:** OrangeHRM Public Demo

**Environment:** Public Web Demo

### Browser

Primary browser:

- Google Chrome

Other browsers may be used when cross-browser behavior needs to be investigated.

### Platform

- Windows
- Desktop environment

---

## 8. Test Data

Test data may include:

- Valid credentials
- Invalid credentials
- Empty inputs
- Boundary values
- Invalid input formats
- Employee information
- Leave information
- Attendance/time information
- Recruitment information
- Other data required by individual modules

Test data will be documented within the relevant Test Cases when necessary.

---

## 9. Tools

| Tool | Purpose |
|---|---|
| Qase | Test Case management and Test Execution |
| Jira | Defect management |
| GitHub | Project documentation and version control |
| Chrome DevTools | Web inspection and troubleshooting |
| Screenshots / Screen Recording | Defect evidence |

---

## 10. Defect Management

When a Test Case fails, the behavior will first be investigated to determine whether it represents:

- A confirmed **Defect**
- Expected behavior
- An **Observation**
- An issue requiring further investigation

Confirmed defects will be documented in Jira.

A defect report should contain, where applicable:

- Summary
- Environment
- Preconditions
- Steps to Reproduce
- Test Data
- Expected Result
- Actual Result
- Severity
- Priority
- Evidence
- Related Test Case

The objective is to make every reported defect clear, reproducible, and actionable.

---

## 11. Entry Criteria

Testing can begin when:

- The relevant feature is accessible.
- The feature can be explored in the test environment.
- Required test data is available.
- The related User Story has been defined.
- Acceptance Criteria have been defined.
- Test Cases have been created and reviewed.

---

## 12. Exit Criteria

Testing for a feature/module can be considered complete when:

- Planned Test Cases have been executed.
- Failed Test Cases have been investigated.
- Confirmed defects have been documented.
- Test results have been recorded.
- Relevant observations have been documented.
- The planned coverage level for the feature/module has been completed.

### Overall Project Exit Criteria

The project will be considered complete when:

- All planned Core modules have received full workflow coverage.
- All planned Secondary modules have received their defined functional coverage.
- Basic/Exploratory modules have received their planned coverage.
- Test execution results have been documented.
- Confirmed defects have been reported.
- The Final Test Summary Report has been prepared.

---

## 13. Risks

Potential project risks include:

- Public demo becoming unavailable.
- Test data being reset or changed.
- Existing defects affecting dependent functionality.
- Demo environment behaving differently from a production environment.
- Lack of explicit requirements for some features.
- Some functionality being unavailable in the public demo.
- Changes in the demo environment during testing.

---

## 14. Assumptions

The following assumptions are made:

- The OrangeHRM public demo is available during testing.
- The application behavior observed in the demo represents the behavior being tested.
- Required functionality is accessible through the available test environment.
- Where formal requirements are unavailable, expectations will be documented carefully based on observable behavior and reasonable product behavior.
- Testing will be performed manually.
- The project focuses on black-box testing from the user's perspective.

---

## 15. Coverage Strategy

The project will prioritize testing depth according to the following structure:

| Priority | Coverage Level | Modules | Testing Depth |
|---|---|---|---|
| 🔴 Core | Full Workflow | Login, Dashboard, PIM, Leave, Time, Recruitment, Admin | High |
| 🟡 Secondary | Core Features | My Info, Performance, Claim, Directory | Medium |
| 🟢 Basic | Basic / Exploratory | Maintenance, Buzz | Low |

### Coverage Principle

The objective is **not** to create an arbitrary number of Test Cases.

Instead, the goal is to achieve meaningful coverage by identifying:

- Main workflows
- Important business rules
- Positive paths
- Negative paths
- Validation rules
- Boundary conditions
- Navigation behavior
- Role/permission behavior
- Important dependencies
- Exploratory risks

The Core modules should receive the largest amount of analysis and testing effort.

---

## 16. Deliverables

The project will produce the following deliverables:

1. **Test Plan**
2. **User Stories**
3. **Acceptance Criteria**
4. **Test Cases**
5. **Test Execution Results**
6. **Defect Reports**
7. **Final Test Summary Report**
8. **GitHub Project Documentation**

---

## 17. Project Workflow

```text
                    Test Plan
                        ↓
                  User Stories
                        ↓
              Acceptance Criteria
                        ↓
                   Test Cases
                        ↓
                Test Execution
                        ↓
                  ┌─────┴─────┐
                  ↓           ↓
                PASS         FAIL
                  ↓           ↓
             Document     Investigate
                              ↓
                     ┌────────┴────────┐
                     ↓                 ↓
                   Bug            Observation
                     ↓                 ↓
                Jira Report       Document