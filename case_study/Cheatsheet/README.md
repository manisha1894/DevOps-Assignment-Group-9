# Testing Cheatsheet

## 1. Software Testing

Software testing is the process of checking software to find defects and verify that it meets the required requirements.

## 2. Types of Testing

* **Unit Testing** – Tests individual functions or modules.
* **Integration Testing** – Tests interaction between different modules.
* **System Testing** – Tests the complete application.
* **Acceptance Testing** – Checks whether the software meets user/business requirements.
* **Regression Testing** – Ensures that new changes have not broken existing functionality.
* **Smoke Testing** – Basic testing to check whether the build is stable enough for further testing.
* **Sanity Testing** – Quick testing of specific changes or functionality.

## 3. Manual vs Automation Testing

| Manual Testing                    | Automation Testing                      |
| --------------------------------- | --------------------------------------- |
| Tests are performed manually      | Tests are performed using scripts/tools |
| More time-consuming               | Faster for repeated tests               |
| No programming is always required | Usually requires programming            |
| Suitable for exploratory testing  | Suitable for regression testing         |

## 4. Testing in DevOps

Testing is integrated throughout the DevOps lifecycle to detect defects early and improve software quality.

**Plan → Code → Build → Test → Release → Deploy → Operate → Monitor**

## 5. CI/CD Testing

In a CI/CD pipeline, automated tests can run whenever new code is committed.

**Code → Build → Unit Test → Integration Test → Deploy**

Benefits:

* Early bug detection
* Faster feedback
* Reduced manual effort
* Better software quality
* Continuous delivery

## 6. Common Testing Tools

* **Selenium** – Web automation testing
* **JUnit** – Java unit testing
* **PyTest** – Python testing
* **Jenkins** – CI/CD automation
* **Postman** – API testing
* **JMeter** – Performance testing

## 7. Important Testing Terms

* **Test Case:** A set of steps and conditions used to verify a feature.
* **Test Scenario:** A high-level situation or functionality to be tested.
* **Bug/Defect:** An error or unexpected behavior in software.
* **Test Plan:** Document describing the testing strategy and scope.
* **Test Automation:** Using software tools/scripts to execute tests automatically.
