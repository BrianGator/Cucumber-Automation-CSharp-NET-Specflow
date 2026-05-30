# Cucumber & SpecFlow Test Automation for C# .NET

A comprehensive test automation framework demonstrating BDD (Behavior-Driven Development) using Cucumber with SpecFlow in C# .NET. This project showcases professional-grade test automation practices with Gherkin feature files and step definitions.

## 📋 Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Key Features](#key-features)
- [Prerequisites](#prerequisites)
- [Languages & Technologies](#languages--technologies)
- [Cucumber Methodologies Covered](#cucumber-methodologies-covered)
- [How to Use](#how-to-use)
- [Installation](#installation)
- [Running Tests](#running-tests)
- [Project Sections](#project-sections)

---

## Overview

This repository contains a complete SpecFlow test automation suite demonstrating best practices for:
- **Behavior-Driven Development (BDD)** with Gherkin syntax
- **Test Automation** patterns and practices
- **C# .NET** implementation of test steps
- **Scalable** test framework architecture

The project is structured into learning sections (Section 4 through Section 15), each covering different aspects of Cucumber and SpecFlow automation.

---

## Project Structure

```
Cucumber-Automation-CSharp-NET-Specflow/
├── README.md                          # This file
├── Section 4/                         # Initial BDD concepts
├── Section 5/                         # Test structure & organization
├── Section 6/                         # Advanced step definitions
├── Section 7/                         # Data-driven testing
├── Section 8/                         # Hooks & test lifecycle
├── Section 9/                         # Advanced Gherkin scenarios
├── Section 10/                        # Integration testing
├── Section 11/                        # Performance testing
├── Section 12/                        # Error handling & reporting
├── Section 13/                        # Parallel execution
├── Section 14/                        # CI/CD integration
└── Section 15/                        # Best practices & patterns
```

---

## Key Features

✅ **Behavior-Driven Development (BDD)**
- Human-readable Gherkin feature files
- Clear Given-When-Then scenario structure
- Executable specifications

✅ **Professional Test Framework**
- Organized step definitions in C#
- Reusable test components
- Page Object Model support
- Data-driven testing capabilities

✅ **Comprehensive Coverage**
- Unit test automation
- Integration test examples
- End-to-end test scenarios
- API testing demonstrations

✅ **Advanced Testing Patterns**
- Before/After hooks for test setup and teardown
- Scenario context management
- Tag-based test execution
- Parallel test execution

✅ **Reporting & Logging**
- Built-in SpecFlow reporting
- Test execution tracking
- Detailed test result documentation

✅ **Scalable Architecture**
- Modular step definitions
- Feature-based organization
- Easy maintenance and expansion
- Code reusability patterns

---

## Prerequisites

### System Requirements
- **Windows 10/11** or **macOS** or **Linux**
- **.NET Framework** 4.7.2 or higher, OR **.NET Core** 3.1+, OR **.NET 5+**

### Required Software
- **Visual Studio 2019/2022** or **Visual Studio Code**
- **NuGet Package Manager**
- **Git** (for version control)

### Build Tools
- **.NET SDK** (latest stable version recommended)
- **C# 8.0** or higher

---

## Languages & Technologies

### Primary Languages
| Language | Usage | Percentage |
|----------|-------|-----------|
| **C#** | Step Definitions, Test Logic, Framework | 80.9% |
| **Gherkin** | Feature Files, Test Scenarios | 19.1% |

### Core Technologies
- **SpecFlow** - BDD framework for .NET
- **Cucumber** - BDD standard & Gherkin language
- **NUnit/MSTest/xUnit** - Unit testing frameworks
- **Selenium WebDriver** (optional) - Web automation
- **RestSharp** (optional) - API testing

### Key NuGet Packages
```
SpecFlow
SpecFlow.NUnit (or MSTest/xUnit)
Selenium.WebDriver (for web automation)
RestSharp (for API testing)
NLog (for logging)
```

---

## Cucumber Methodologies Covered

### 1. **Gherkin Syntax & Semantics**
   - Feature files structure
   - Scenario definitions
   - Scenario Outline with Examples
   - Background setup

### 2. **Given-When-Then Pattern**
   - Preconditions (Given)
   - User actions (When)
   - Expected outcomes (Then)
   - Supporting clauses (And, But)

### 3. **Step Definitions**
   - Regular expressions in step bindings
   - Step parameters and tables
   - Multiline text handling
   - Step definition reusability

### 4. **Hooks & Lifecycle Management**
   - `[Before]` hooks for setup
   - `[After]` hooks for teardown
   - Test context sharing
   - Scenario context usage

### 5. **Data-Driven Testing**
   - Scenario Outlines
   - Example tables
   - Multiple iteration scenarios

### 6. **Test Organization**
   - Feature file grouping
   - Tag-based organization
   - Scenario filtering

### 7. **Integration & CI/CD**
   - Continuous Integration setup
   - Test execution pipelines
   - Automated test runs
   - Report generation

### 8. **Advanced Patterns**
   - Page Object Model with Gherkin
   - Custom step definitions
   - Error handling in automation
   - Performance testing scenarios

---

## How to Use

### 1. **Clone the Repository**
```bash
git clone https://github.com/BrianGator/Cucumber-Automation-CSharp-NET-Specflow.git
cd Cucumber-Automation-CSharp-NET-Specflow
```

### 2. **Explore Sections**
Start with **Section 4** for fundamentals and progress through sections sequentially:
- Each section builds on previous concepts
- Contains example feature files (`.feature`)
- Includes corresponding step definitions (`.cs`)

### 3. **Review Feature Files**
Each section contains `.feature` files with Gherkin scenarios:
```gherkin
Feature: Example Feature
  Description of what this feature does

  Scenario: Example scenario
    Given a precondition exists
    When I perform an action
    Then I should see the expected result
```

### 4. **Study Step Definitions**
Examine C# step definition files to understand:
- How to bind Gherkin steps to code
- Best practices for test implementation
- Data handling and assertions

### 5. **Run Test Scenarios**
Execute tests through your IDE or command line

---

## Installation

### Option 1: Visual Studio 2022

1. **Open the Solution**
   ```
   File → Open → Project/Solution
   Select the .sln file
   ```

2. **Restore NuGet Packages**
   ```
   Tools → NuGet Package Manager → Manage NuGet Packages for Solution
   Click "Restore"
   ```

3. **Build Solution**
   ```
   Build → Build Solution (Ctrl+Shift+B)
   ```

### Option 2: Command Line (.NET CLI)

```bash
# Restore packages
dotnet restore

# Build project
dotnet build

# Run tests
dotnet test
```

### Option 3: Package Manager Console

```powershell
# Install SpecFlow
Install-Package SpecFlow

# Install test framework (choose one)
Install-Package SpecFlow.NUnit
Install-Package SpecFlow.MSTest
Install-Package SpecFlow.xUnit

# Restore all packages
Update-Package -Reinstall
```

---

## Running Tests

### Using Visual Studio Test Explorer
1. Open **Test Explorer** (Test → Windows → Test Explorer)
2. Click **Run All Tests**
3. View results in the Test Explorer window

### Using SpecFlow Runner
```bash
dotnet test
```

### Running Specific Test
```bash
dotnet test --filter "Category=SmokeTests"
```

### Running with Tags
```bash
# Run only scenarios tagged with @smoke
dotnet test --filter "Tags=smoke"
```

### Generate Reports
```bash
# SpecFlow HTML report
dotnet test -- --logger:"html;LogFileName=TestResults.html"
```

---

## Project Sections

| Section | Topic | Focus |
|---------|-------|-------|
| **Section 4** | BDD Fundamentals | Introduction to Gherkin & SpecFlow |
| **Section 5** | Test Structure | Organizing features and step definitions |
| **Section 6** | Advanced Steps | Complex step definitions and validations |
| **Section 7** | Data-Driven Tests | Scenario Outlines and example tables |
| **Section 8** | Hooks & Lifecycle | Before/After hooks and context management |
| **Section 9** | Advanced Scenarios | Complex Gherkin patterns |
| **Section 10** | Integration Tests | Multi-component testing |
| **Section 11** | Performance | Load and performance testing |
| **Section 12** | Error Handling | Exception handling and reporting |
| **Section 13** | Parallel Execution | Running tests in parallel |
| **Section 14** | CI/CD Integration | GitHub Actions, Azure Pipelines setup |
| **Section 15** | Best Practices | Patterns, anti-patterns, and recommendations |

---

## Best Practices

### ✅ DO:
- Keep feature files focused and readable
- Use descriptive scenario names
- Reuse step definitions across scenarios
- Maintain a clear folder structure
- Use tags for organization and filtering
- Keep steps independent and atomic
- Document complex step logic

### ❌ DON'T:
- Hardcode test data in step definitions
- Create overly complex Gherkin scenarios
- Mix multiple concerns in a single step
- Ignore test execution failures
- Create duplicate step definitions
- Use implementation details in feature files

---

## Contributing

Contributions are welcome! Please:
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

---

## Resources

- [SpecFlow Official Documentation](https://specflow.org/documentation/)
- [Cucumber Gherkin Reference](https://cucumber.io/docs/gherkin/)
- [C# Automation Best Practices](https://docs.microsoft.com/en-us/dotnet/)
- [BDD Principles](https://cucumber.io/docs/bdd/)

---

## License

This project is open source and available for educational purposes.

---

## Support

For questions or issues:
- Review the relevant section in the repository
- Check SpecFlow documentation
- Refer to inline code comments and examples

---

**Happy Testing! 🚀**

*Last Updated: 2026-05-30*
*Framework: SpecFlow for .NET*
*Languages: C# & Gherkin*
