---
layout: standard
order: 1
title: test coverage
date: 2025-07-08
id: SEGAS-00017
tags:
- Developer Testing 
- Quality engineering
  
---
## Test Coverage

Appropriate test coverage is a fundamental practice in Quality Engineering that goes beyond simply measuring the percentage of code lines executed by tests.

It's principle is to ensure the tests provide meaningful validation of the requirement, reduce the risk of defects, and ultimately contribute to higher-quality software. Focusing on the principles of effective code coverage—such as prioritising behaviour over mere lines of code, targeting critical paths and edge cases, and integrating testing seamlessly into the development workflow - teams will realise improved outcomes.

Outcomes include increased confidence in code changes, earlier detection of bugs, reduced technical debt, and improved maintainability. Effective code coverage enables Quality Engineers to build robust and reliable software, enabling a culture of quality and continuous improvement.

---

## Requirements

- [You MUST have a minimum of 80% code coverage](#you-must-have-a-minimum-of-80-code-coverage)
- [You MUST implement static code vulnerability scans as well as dynamic analysis to identify security issues within the code](#you-must-implement-static-code-vulnerability-scans-as-well-as-dynamic-analysis-to-identify-security-issues-within-the-code)
- [You MUST prioritise testing coverage on the expected behaviour of the code, including edge cases and boundary conditions](#you-must-prioritise-testing-coverage-on-the-expected-behaviour-of-the-code-including-edge-cases-and-boundary-conditions)
- [You MUST Prioritise testing critical or high-risk areas of the application](#you-must-prioritise-testing-critical-or-high-risk-areas-of-the-application)
- [You MUST prioritise achieving coverage target for new code changes, legacy system unit tests should be secondary](#you-must-prioritise-achieving-coverage-target-for-new-code-changes-legacy-system-unit-tests-should-be-secondary)
- [You MUST implement code coverage tools integrated into CI/CD pipelines for continuous measurement](#you-must-implement-code-coverage-tools-integrated-into-cicd-pipelines-for-continuous-measurement)
- [You MUST have Test Coverage Metrics that emphasise a holistic approach to Quality Engineering](#you-must-have-test-coverage-metrics-that-emphasise-a-holistic-approach-to-quality-engineering)

### You MUST have a minimum of 80% code coverage

Maintaining a minimum of 80% code coverage ensures that a significant portion of the codebase is tested, reducing the risk of undetected defects. Utilise options like AWS CodeBuild to execute tests with coverage tools such as Jacoco or Istanbul, and integrate AWS CodePipeline to mandate an 80% coverage requirement before code merging or deployment. Furthermore, AWS Lambda can trigger alerts or prevent deployments if coverage drops below this 80% threshold, thereby ensuring continuous quality checks. This threshold helps improve software reliability, maintainability, and overall quality by verifying that critical logic paths, functions, and features are covered by automated tests. while 100% coverage is not always practical, setting a standard of 80% encourages consistency testing practices without excessive overhead.

### You MUST implement static code vulnerability scans as well as dynamic analysis to identify security issues within the code

Implementing static code vulnerability scans is essential for proactively identifying security weakness within the codebase. Integrate static code analysis tools like SonarQube into the CI/CD pipeline to automatically scan source code, dependencies, and configurations for security vulnerabilities. Establish automated feedback loops to promptly notify developers of identified security risks, enabling them to address these vulnerabilities before code merges or deployments. These scans analyse source code, configuration files, and dependencies to detect vulnerabilities such as insecure coding practices, injection risks, and potential exploits before they reach production. By integrating static code analysis tools into the development pipeline, teams can address security issues early, enhance compliance with security standards, and reduce the risk of beaches or data exposure.

### You MUST prioritise testing coverage on the expected behaviour of the code, including edge cases and boundary conditions

Prioritise testing coverage based on the expected behaviour of the code, so that tests align with real-world usage scenarios, reducing the risk of undetected issues. Develop a testing strategy that prioritises real-world scenarios, encompassing normal, edge, and boundary conditions to ensure comprehensive coverage of the application's most critical parts. Implement test automation to consistently validate these key scenarios during each development cycle, improving both efficiency and reliability. This approach emphasises functional validation under normal conditions, as well as covering edge cases and boundary conditions, where software is most prone to failure. By focusing on these critical areas, teams can improve software robustness, prevent unexpected failures, and enhance user experience, ultimately leading to higher-quality and more reliable applications.

### You MUST Prioritise testing critical or high-risk areas of the application

Focussing test coverage on critical or high-risk areas of the application so that the most impactful and vulnerable components are thoroughly validated. Develop a risk-based testing strategy that prioritises the most impactful and vulnerable components, ensuring critical areas like core functionalities and security-sensitive features are thoroughly tested. Employ automated testing to consistently validate these high-risk areas, maintaining focus on these components throughout the development lifecycle. High-risk areas include core functionalities, security-sensitive features, complex logic, and components with a history of defects. By prioritising testing in these areas, teams should mitigate potential failures, reduce business risks, and enhance software reliability, ultimately leading to a more stable and resilient application.

### You MUST prioritise achieving coverage target for new code changes, legacy system unit tests should be secondary

Test coverage targets for new code changes is crucial for maintaining software quality and preventing defects from being introduced into the system. Prioritise achieving test coverage for new code changes to maintain high software quality by ensuring new code meets quality standards from the beginning, while treating legacy system unit tests as secondary and focusing primarily on verifying new or modified code, acknowledging that legacy code may initially only require refactoring before effective testing. This approach balances test efficiency code maintainability, and risk mitigation, fostering a more sustainable and scalable development process.

### You MUST implement code coverage tools integrated into CI/CD pipelines for continuous measurement

Integrating code coverage tools into CI/CD pipelines enables continuous measurement and monitoring of test coverage throughout the development lifecycle. Automated coverage analysis ensures that every code change is evaluated for test completeness, preventing untested or insufficiently tested code from being deployed. This integration promotes early defect detection, enforces quality standards, and streamlines the development workflow, leading to more reliable software releases with minimal manual intervention.

### You MUST have Test Coverage Metrics that emphasise a holistic approach to Quality Engineering

Test coverage metrics should reflect a holistic approach to Quality Engineering, focussing not just on percentage-based coverage but also on the effectiveness of tests in detecting defects, covering critical functionality, and addressing edge cases. By emphasising meaningful coverage rather than just numerical targets, teams can achieve higher software reliability, maintainability, and long-term quality assurance:

- % Unit tests v %Integration v % E2E tests
---
