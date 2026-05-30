# Cucumber & SpecFlow Test Automation for C# .NET

A comprehensive test automation framework demonstrating BDD (Behavior-Driven Development) using Cucumber with SpecFlow in C# .NET. This project showcases professional-grade test automation practices with complete coding examples and best practices guide.

## 📋 Table of Contents

### Getting Started
- [Overview](#overview)
- [Project Structure](#project-structure)
- [Key Features](#key-features)
- [Prerequisites](#prerequisites)

### Setup & Installation
- [Languages & Technologies](#languages--technologies)
- [Installation Guide](#installation)
- [Running Tests](#running-tests)

### Learning Path
- [Project Sections](#project-sections)
- [Cucumber Methodologies Covered](#cucumber-methodologies-covered)
- [How to Use](#how-to-use)

### Development Guide
- [SpecFlow & Cucumber Coding Guide](#specflow--cucumber-coding-guide)
  - [Gherkin Feature Files](#gherkin-feature-files)
  - [Step Definitions](#step-definitions)
  - [Hooks & Test Lifecycle](#hooks--test-lifecycle)
  - [Data-Driven Testing](#data-driven-testing-guide)
  - [Advanced Patterns](#advanced-patterns)
  - [Common Pitfalls](#common-pitfalls)
- [Best Practices](#best-practices)
- [Code Examples & Tips](#code-examples--tips)

### Reference
- [Resources](#resources)
- [Contributing](#contributing)
- [Support](#support)

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
│   ├── Features/                      # .feature files
│   ├── StepDefinitions/               # Step definition files
│   └── Hooks/                         # Before/After hooks
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

## How to Use

### 1. **Clone the Repository**
```bash
git clone https://github.com/BrianGator/Cucumber-Automation-CSharp-NET-Specflow.git
cd Cucumber-Automation-CSharp-NET-Specflow
```

### 2. **Explore Sections**
Start with **[Section 4](#section-4-bdd-fundamentals)** for fundamentals and progress through sections sequentially:
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

## Project Sections

| Section | Topic | Focus |
|---------|-------|-------|
| **[Section 4](#section-4-bdd-fundamentals)** | BDD Fundamentals | Introduction to Gherkin & SpecFlow |
| **[Section 5](#section-5-test-structure)** | Test Structure | Organizing features and step definitions |
| **[Section 6](#section-6-advanced-step-definitions)** | Advanced Steps | Complex step definitions and validations |
| **[Section 7](#section-7-data-driven-testing)** | Data-Driven Tests | Scenario Outlines and example tables |
| **[Section 8](#section-8-hooks--lifecycle)** | Hooks & Lifecycle | Before/After hooks and context management |
| **[Section 9](#section-9-advanced-scenarios)** | Advanced Scenarios | Complex Gherkin patterns |
| **[Section 10](#section-10-integration-tests)** | Integration Tests | Multi-component testing |
| **[Section 11](#section-11-performance-testing)** | Performance | Load and performance testing |
| **[Section 12](#section-12-error-handling)** | Error Handling | Exception handling and reporting |
| **[Section 13](#section-13-parallel-execution)** | Parallel Execution | Running tests in parallel |
| **[Section 14](#section-14-cicd-integration)** | CI/CD Integration | GitHub Actions, Azure Pipelines setup |
| **[Section 15](#section-15-best-practices)** | Best Practices | Patterns, anti-patterns, and recommendations |

### Section 4: BDD Fundamentals
Introduction to Gherkin syntax and basic SpecFlow setup. Learn the Given-When-Then pattern.

### Section 5: Test Structure
Organizing features and step definitions following best practices.

### Section 6: Advanced Step Definitions
Complex step definitions with parameters, tables, and multiline arguments.

### Section 7: Data-Driven Testing
Using Scenario Outlines and example tables for parametrized testing.

### Section 8: Hooks & Lifecycle
Managing test setup, teardown, and scenario context.

### Section 9: Advanced Scenarios
Complex Gherkin patterns and scenario composition.

### Section 10: Integration Tests
Multi-component and integration testing scenarios.

### Section 11: Performance Testing
Performance benchmarking and load testing patterns.

### Section 12: Error Handling
Exception handling, logging, and error reporting strategies.

### Section 13: Parallel Execution
Running tests in parallel for faster execution.

### Section 14: CI/CD Integration
GitHub Actions and Azure Pipelines integration examples.

### Section 15: Best Practices
Comprehensive patterns, anti-patterns, and recommendations.

---

## SpecFlow & Cucumber Coding Guide

This section provides comprehensive coding examples and best practices for SpecFlow and Cucumber development in C# .NET.

---

### Gherkin Feature Files

#### ✅ Example 1: Basic Scenario

```gherkin
Feature: User Login
  As a user
  I want to log in to the application
  So that I can access my account

  Background:
    Given the login page is displayed
    And the user database is initialized

  Scenario: Successful login with valid credentials
    Given I have entered username "john.doe" and password "SecurePass123"
    When I click the login button
    Then I should be redirected to the dashboard
    And I should see a welcome message for "john.doe"

  Scenario: Failed login with invalid credentials
    Given I have entered username "invalid.user" and password "WrongPassword"
    When I click the login button
    Then I should remain on the login page
    And I should see an error message "Invalid credentials"
```

**Key Points:**
- Use **Background** for common setup steps
- Keep scenario titles descriptive and concise
- Use **Given-When-Then** structure consistently
- Include both positive and negative scenarios

#### ✅ Example 2: Scenario Outline (Data-Driven)

```gherkin
Feature: Order Processing
  
  Scenario Outline: Process different types of orders
    Given I have a shopping cart with value "<cartValue>"
    When I apply coupon code "<couponCode>"
    And I proceed to checkout
    Then the final amount should be "<finalAmount>"
    And the discount applied should be "<discountPercent>"

    Examples:
      | cartValue | couponCode  | finalAmount | discountPercent |
      | $100.00   | SAVE10      | $90.00      | 10%             |
      | $250.00   | SAVE25      | $187.50     | 25%             |
      | $50.00    | SAVE5       | $47.50      | 5%              |
      | $1000.00  | VIP50       | $500.00     | 50%             |
```

**Key Points:**
- Use **Scenario Outline** for testing multiple scenarios with different data
- Define **Examples** tables with clear header names
- Parameters are enclosed in angle brackets `<parameterName>`
- Each row executes as a separate test

#### ✅ Example 3: Tables in Steps

```gherkin
Feature: Inventory Management

  Scenario: Add multiple items to inventory
    Given the inventory system is started
    When I add the following items:
      | ItemName      | Quantity | Price  |
      | Laptop        | 5        | 999.99 |
      | Monitor       | 10       | 299.99 |
      | Keyboard      | 25       | 79.99  |
      | Mouse         | 50       | 29.99  |
    Then the total inventory value should be calculated correctly
    And each item should be stored in the database

  Scenario: Validate item specifications
    Given I have items with the following details:
      | ItemCode | Name     | Category    | InStock |
      | LAP001   | MacBook  | Computers   | true    |
      | MON001   | Dell U27 | Monitors    | true    |
      | KBD001   | Logitech | Peripherals | false   |
    Then all items should be properly categorized
```

**Key Points:**
- Use **Data Tables** for complex input data
- Headers become column identifiers
- Useful for bulk operations and validations
- Improves readability compared to long steps

---

### Step Definitions

#### ✅ Example 1: Basic Step Definitions

```csharp
using TechTalk.SpecFlow;
using NUnit.Framework;

[Binding]
public class UserLoginSteps
{
    private string _username;
    private string _password;
    private string _actualError;
    private bool _loginSuccessful;

    [Given(@"I have entered username ""([^""]*)"" and password ""([^""]*)""")]
    public void GivenIHaveEnteredUsernameAndPassword(string username, string password)
    {
        _username = username;
        _password = password;
        // Store credentials for login attempt
    }

    [When(@"I click the login button")]
    public void WhenIClickTheLoginButton()
    {
        // Simulate login
        _loginSuccessful = ValidateCredentials(_username, _password);
        if (!_loginSuccessful)
        {
            _actualError = "Invalid credentials";
        }
    }

    [Then(@"I should be redirected to the dashboard")]
    public void ThenIShouldBeRedirectedToTheDashboard()
    {
        Assert.IsTrue(_loginSuccessful, "Login was not successful");
    }

    [Then(@"I should see an error message ""([^""]*)""")]
    public void ThenIShouldSeeAnErrorMessage(string expectedError)
    {
        Assert.AreEqual(expectedError, _actualError, "Error message does not match");
    }

    // Helper method
    private bool ValidateCredentials(string username, string password)
    {
        return username == "john.doe" && password == "SecurePass123";
    }
}
```

**Key Points:**
- Use **[Binding]** attribute on step definition classes
- Use **regex patterns** in `[Given]`, `[When]`, `[Then]` attributes
- Extract parameters from Gherkin steps using **capture groups**
- Keep step definitions focused and testable

#### ✅ Example 2: Table Parameter Handling

```csharp
using TechTalk.SpecFlow;
using NUnit.Framework;

[Binding]
public class InventorySteps
{
    private List<InventoryItem> _addedItems;

    [When(@"I add the following items:")]
    public void WhenIAddTheFollowingItems(Table table)
    {
        _addedItems = new List<InventoryItem>();

        // Convert table rows to objects
        foreach (var row in table.Rows)
        {
            var item = new InventoryItem
            {
                ItemName = row["ItemName"],
                Quantity = int.Parse(row["Quantity"]),
                Price = decimal.Parse(row["Price"])
            };

            _addedItems.Add(item);
            // Add to inventory system
            AddToInventory(item);
        }
    }

    [Then(@"the total inventory value should be calculated correctly")]
    public void ThenTheTotalInventoryValueShouldBeCalculatedCorrectly()
    {
        decimal totalValue = _addedItems.Sum(x => x.Quantity * x.Price);
        decimal expectedTotal = (5 * 999.99m) + (10 * 299.99m) + (25 * 79.99m) + (50 * 29.99m);
        
        Assert.AreEqual(expectedTotal, totalValue, 0.01m, "Total inventory value is incorrect");
    }

    private void AddToInventory(InventoryItem item)
    {
        // Implementation to add item to inventory
    }
}

public class InventoryItem
{
    public string ItemName { get; set; }
    public int Quantity { get; set; }
    public decimal Price { get; set; }
}
```

**Key Points:**
- Use **Table** parameter type to receive Gherkin data tables
- Access columns using **row["ColumnName"]**
- Convert string values to appropriate types
- Iterate through rows for bulk operations

#### ✅ Example 3: Multiline Text and Complex Parameters

```csharp
using TechTalk.SpecFlow;
using NUnit.Framework;

[Binding]
public class DocumentSteps
{
    private string _documentContent;
    private string _documentTitle;

    [Given(@"I create a document with title ""([^""]*)""")]
    public void GivenICreateADocumentWithTitle(string title)
    {
        _documentTitle = title;
        _documentContent = string.Empty;
    }

    [When(@"I add the following content:")]
    public void WhenIAddTheFollowingContent(string content)
    {
        _documentContent = content;
        // content can be multiline from the feature file
    }

    [Then(@"the document should contain:")]
    public void ThenTheDocumentShouldContain(string expectedContent)
    {
        Assert.That(_documentContent, Does.Contain(expectedContent), 
            "Document does not contain expected content");
    }

    [Then(@"the word count should be (\d+)")]
    public void ThenTheWordCountShouldBe(int expectedWordCount)
    {
        int actualWordCount = _documentContent.Split(new[] { ' ', '\n', '\r' }, 
            System.StringSplitOptions.RemoveEmptyEntries).Length;
        
        Assert.AreEqual(expectedWordCount, actualWordCount, 
            "Word count does not match");
    }
}
```

**Usage in Feature File:**
```gherkin
Scenario: Create document with multiline content
  Given I create a document with title "My Report"
  When I add the following content:
    """
    This is a comprehensive report
    with multiple paragraphs.
    
    It contains detailed information
    about the project status.
    """
  Then the document should contain:
    """
    comprehensive report
    """
  And the word count should be 20
```

**Key Points:**
- Use **multiline strings** (triple quotes) for long text
- Use **(\d+)** regex for numeric parameters
- Use **[^""]*** regex for text without quotes
- Support complex data scenarios

---

### Hooks & Test Lifecycle

#### ✅ Example 1: Before/After Hooks

```csharp
using TechTalk.SpecFlow;
using NUnit.Framework;

[Binding]
public class Hooks
{
    private TestContext _testContext;

    // Runs before each scenario
    [Before]
    public void BeforeScenario(ScenarioContext scenarioContext)
    {
        _testContext = new TestContext();
        _testContext.Initialize();
        
        // Log scenario start
        Console.WriteLine($"Starting scenario: {scenarioContext.ScenarioInfo.Title}");
    }

    // Runs after each scenario
    [After]
    public void AfterScenario(ScenarioContext scenarioContext)
    {
        // Cleanup
        _testContext.Cleanup();
        
        // Log test result
        Console.WriteLine($"Scenario result: {scenarioContext.TestError?.Message ?? "PASSED"}");
    }

    // Hook with tags
    [Before("@database")]
    public void BeforeDatabaseTests()
    {
        // Initialize database connection
        Console.WriteLine("Setting up database connection");
    }

    [After("@database")]
    public void AfterDatabaseTests()
    {
        // Close database connection
        Console.WriteLine("Closing database connection");
    }

    // Hook with order - runs first
    [Before(Order = 1)]
    public void FirstBeforeHook()
    {
        Console.WriteLine("This runs first");
    }

    // Hook with order - runs second
    [Before(Order = 2)]
    public void SecondBeforeHook()
    {
        Console.WriteLine("This runs second");
    }
}

public class TestContext
{
    public void Initialize()
    {
        // Initialize test resources
    }

    public void Cleanup()
    {
        // Release resources
    }
}
```

#### ✅ Example 2: ScenarioContext for Sharing Data

```csharp
using TechTalk.SpecFlow;

[Binding]
public class UserContextSteps
{
    private readonly ScenarioContext _scenarioContext;

    // Inject ScenarioContext through constructor
    public UserContextSteps(ScenarioContext scenarioContext)
    {
        _scenarioContext = scenarioContext;
    }

    [Given(@"I have a user with email ""([^""]*)""")]
    public void GivenIHaveAUserWithEmail(string email)
    {
        var user = new User { Email = email };
        
        // Store user in context for access in other steps
        _scenarioContext["CurrentUser"] = user;
    }

    [When(@"I update the user profile")]
    public void WhenIUpdateTheUserProfile()
    {
        // Retrieve user from context
        var user = _scenarioContext["CurrentUser"] as User;
        
        if (user != null)
        {
            user.LastUpdated = DateTime.Now;
            _scenarioContext["CurrentUser"] = user;
        }
    }

    [Then(@"the user should have an updated profile")]
    public void ThenTheUserShouldHaveAnUpdatedProfile()
    {
        var user = _scenarioContext["CurrentUser"] as User;
        
        Assert.IsNotNull(user?.LastUpdated, "User profile was not updated");
    }
}

public class User
{
    public string Email { get; set; }
    public DateTime? LastUpdated { get; set; }
}
```

**Key Points:**
- Use **ScenarioContext** to share data between steps
- Inject context through constructor
- Access with **scenarioContext[key]** syntax
- Store complex objects for scenario-wide access

---

### Data-Driven Testing Guide

#### ✅ Example 1: Scenario Outline Best Practices

```gherkin
Feature: Payment Processing

  Scenario Outline: Calculate shipping costs based on location and weight
    Given I have a package weighing "<weight>" pounds
    And the destination is "<location>"
    When I calculate shipping cost
    Then the cost should be "$<shippingCost>"

    Examples: Domestic Shipping
      | weight | location      | shippingCost |
      | 5      | New York      | 15.99        |
      | 10     | California    | 22.99        |
      | 2      | Texas         | 10.99        |

    Examples: International Shipping
      | weight | location      | shippingCost |
      | 5      | Canada        | 35.99        |
      | 10     | Mexico        | 42.99        |
      | 2      | UK            | 55.99        |
```

**Key Points:**
- Use **multiple Examples blocks** for different test scenarios
- Label examples with **descriptive names**
- Each examples block runs separately with same scenario
- Improves test readability and maintenance

#### ✅ Example 2: Implementing Scenario Outline Steps

```csharp
using TechTalk.SpecFlow;
using NUnit.Framework;

[Binding]
public class ShippingSteps
{
    private decimal _packageWeight;
    private string _destination;
    private decimal _calculatedCost;

    [Given(@"I have a package weighing ""([^""]*)"" pounds")]
    public void GivenIHaveAPackageWeighing(string weight)
    {
        _packageWeight = decimal.Parse(weight);
    }

    [Given(@"the destination is ""([^""]*)""")]
    public void GivenTheDestinationIs(string location)
    {
        _destination = location;
    }

    [When(@"I calculate shipping cost")]
    public void WhenICalculateShippingCost()
    {
        _calculatedCost = CalculateShipping(_packageWeight, _destination);
    }

    [Then(@"the cost should be ""([^""]*)""")]
    public void ThenTheCostShouldBe(string expectedCost)
    {
        decimal expected = decimal.Parse(expectedCost.Replace("$", ""));
        Assert.AreEqual(expected, _calculatedCost, 0.01m, 
            $"Shipping cost mismatch for {_destination}");
    }

    private decimal CalculateShipping(decimal weight, string location)
    {
        // Shipping rate calculation logic
        decimal baseRate = location.Contains("International") ? 30m : 10m;
        return baseRate + (weight * 2);
    }
}
```

---

### Advanced Patterns

#### ✅ Example 1: Page Object Model Pattern

```csharp
// LoginPage.cs
public class LoginPage
{
    private readonly IWebDriver _driver;

    public LoginPage(IWebDriver driver)
    {
        _driver = driver;
    }

    // Page Elements
    public IWebElement UsernameField => _driver.FindElement(By.Id("username"));
    public IWebElement PasswordField => _driver.FindElement(By.Id("password"));
    public IWebElement LoginButton => _driver.FindElement(By.Id("login-btn"));
    public IWebElement ErrorMessage => _driver.FindElement(By.ClassName("error-message"));

    // Page Methods
    public void EnterUsername(string username)
    {
        UsernameField.Clear();
        UsernameField.SendKeys(username);
    }

    public void EnterPassword(string password)
    {
        PasswordField.Clear();
        PasswordField.SendKeys(password);
    }

    public void ClickLogin()
    {
        LoginButton.Click();
    }

    public bool IsErrorDisplayed()
    {
        return ErrorMessage.Displayed;
    }

    public string GetErrorText()
    {
        return ErrorMessage.Text;
    }
}

// LoginSteps.cs using Page Object
[Binding]
public class LoginStepsWithPOM
{
    private readonly ScenarioContext _scenarioContext;
    private LoginPage _loginPage;

    public LoginStepsWithPOM(ScenarioContext scenarioContext)
    {
        _scenarioContext = scenarioContext;
    }

    [Given(@"I am on the login page")]
    public void GivenIAmOnTheLoginPage()
    {
        var driver = _scenarioContext["WebDriver"] as IWebDriver;
        _loginPage = new LoginPage(driver);
    }

    [Given(@"I have entered valid credentials")]
    public void GivenIHaveEnteredValidCredentials()
    {
        _loginPage.EnterUsername("testuser");
        _loginPage.EnterPassword("password123");
    }

    [When(@"I click login")]
    public void WhenIClickLogin()
    {
        _loginPage.ClickLogin();
    }
}
```

#### ✅ Example 2: Custom Hook for Test Data Management

```csharp
using TechTalk.SpecFlow;

[Binding]
public class TestDataHooks
{
    private readonly ScenarioContext _scenarioContext;
    private DatabaseConnection _dbConnection;

    public TestDataHooks(ScenarioContext scenarioContext)
    {
        _scenarioContext = scenarioContext;
    }

    [Before("@requiresTestData")]
    public void SetupTestData()
    {
        _dbConnection = new DatabaseConnection();
        
        // Create test users
        var testUser = new User 
        { 
            Id = Guid.NewGuid(),
            Email = "test@example.com",
            Username = "testuser"
        };
        
        _dbConnection.InsertUser(testUser);
        
        // Store in context for use in steps
        _scenarioContext["TestUser"] = testUser;
    }

    [After("@requiresTestData")]
    public void CleanupTestData()
    {
        // Delete test data
        var testUser = _scenarioContext["TestUser"] as User;
        if (testUser != null)
        {
            _dbConnection.DeleteUser(testUser.Id);
        }
        
        _dbConnection.Dispose();
    }
}

public class DatabaseConnection : IDisposable
{
    public void InsertUser(User user) { /* implementation */ }
    public void DeleteUser(Guid userId) { /* implementation */ }
    public void Dispose() { /* cleanup */ }
}
```

---

### Common Pitfalls

#### ❌ Pitfall 1: UI Implementation Details in Feature Files

```gherkin
// BAD - Implementation details
Scenario: Bad Implementation
  Given I click on the element with id "login-button-xyz-123"
  When I wait 5 seconds
  Then I should see the value in input field with class "form-input-primary"

// GOOD - Business language
Scenario: Good Business Language
  Given I am on the login page
  When I click the login button
  Then I should see the dashboard
```

#### ❌ Pitfall 2: Duplicate Step Definitions

```csharp
// BAD - Duplicate steps
[Given("I navigate to the home page")]
public void Step1() { Navigate("home"); }

[Given("I navigate to home")]
public void Step2() { Navigate("home"); }

// GOOD - Reusable step
[Given(@"I navigate to the (home|dashboard|profile) page")]
public void NavigateToPage(string page)
{
    Navigate(page);
}
```

#### ❌ Pitfall 3: Hardcoded Test Data

```csharp
// BAD - Hardcoded data
[Given("I have a user")]
public void HardcodedUser()
{
    CreateUser("john.doe", "password123", "john@example.com");
}

// GOOD - Parameterized data
[Given(@"I have a user with email ""([^""]*)""")]
public void ParametrizedUser(string email)
{
    CreateUser("testuser", "password123", email);
}
```

#### ❌ Pitfall 4: Too Many Assertions in One Step

```csharp
// BAD - Multiple assertions in one step
[Then("everything should be correct")]
public void BadAssertions()
{
    Assert.AreEqual(expected1, actual1);
    Assert.AreEqual(expected2, actual2);
    Assert.AreEqual(expected3, actual3);
}

// GOOD - One assertion per step
[Then("the username should be displayed")]
public void UsernameDisplayed()
{
    Assert.AreEqual("john.doe", GetDisplayedUsername());
}

[Then("the email should be verified")]
public void EmailVerified()
{
    Assert.IsTrue(IsEmailVerified());
}
```

---

## Best Practices

### ✅ DO:

- **Keep feature files focused and readable**
  ```gherkin
  Scenario: Single, well-defined behavior
    Given clear preconditions
    When one action is performed
    Then verify specific outcome
  ```

- **Use descriptive scenario names**
  ```gherkin
  Scenario: User can successfully login with valid credentials
  ✓ Better: Specific behavior
  ✗ Worse: Scenario 1
  ```

- **Reuse step definitions across scenarios**
  - Use regex patterns for parameterization
  - Avoid creating similar steps with different names

- **Maintain a clear folder structure**
  - Organize by feature or domain
  - Keep related steps together

- **Use tags for organization and filtering**
  ```gherkin
  @smoke @critical @web
  Scenario: Important feature
  ```

- **Keep steps independent and atomic**
  - Each step should be self-contained
  - Avoid inter-step dependencies

- **Document complex step logic**
  ```csharp
  // Calculate compound interest with specified rate
  [When(@"I calculate interest at (\d+)% for (\d+) years")]
  public void CalculateInterest(decimal rate, int years)
  {
      // Implementation with comments
  }
  ```

### ❌ DON'T:

- **Hardcode test data in step definitions**
  - Use parameters from feature files
  - Use external data sources

- **Create overly complex Gherkin scenarios**
  - Keep scenarios focused
  - One behavior per scenario

- **Mix multiple concerns in a single step**
  - Login + verify + check email = bad
  - Each step does one thing

- **Ignore test execution failures**
  - Investigate root causes
  - Fix flaky tests

- **Create duplicate step definitions**
  - Use regex to generalize
  - Maintain one source of truth

- **Use implementation details in feature files**
  - Focus on business behavior
  - Hide technical details

---

## Code Examples & Tips

### Tip 1: Regex Patterns for Step Parameters

```csharp
// Exact text in quotes
[Given(@"I enter ""([^""]*)""")]
public void EnterText(string text) { }

// Numbers
[Given(@"I have (\d+) items")]
public void HaveItems(int count) { }

// Decimal numbers
[Given(@"the price is £([\d.]+)")]
public void SetPrice(decimal price) { }

// Optional text
[Given(@"I am (.+?)")]
public void SetStatus(string status) { }

// Multiple alternatives
[Given(@"I navigate to (home|dashboard|profile)")]
public void Navigate(string page) { }
```

### Tip 2: Table Processing Efficiently

```csharp
[When(@"I process the following:")]
public void ProcessTable(Table table)
{
    // Method 1: Direct row iteration
    foreach (var row in table.Rows)
    {
        string name = row["Name"];
        int age = int.Parse(row["Age"]);
    }

    // Method 2: Convert to objects
    var items = table.CreateSet<TestItem>();
    foreach (var item in items)
    {
        // Work with strongly-typed objects
    }

    // Method 3: Key-value dictionary
    foreach (var row in table.Rows)
    {
        var dict = row.Keys.ToDictionary(k => k, k => row[k]);
    }
}
```

### Tip 3: Using ScenarioContext Effectively

```csharp
[Binding]
public class ContextExample
{
    private readonly ScenarioContext _context;

    public ContextExample(ScenarioContext context)
    {
        _context = context;
    }

    [Given("I store a value")]
    public void StoreValue()
    {
        _context["key"] = "value";
    }

    [Then("I retrieve the value")]
    public void RetrieveValue()
    {
        var value = _context.Get<string>("key");
        Assert.AreEqual("value", value);
    }

    [Then("I check if key exists")]
    public void CheckKey()
    {
        bool exists = _context.ContainsKey("key");
    }
}
```

### Tip 4: Exception Handling in Steps

```csharp
[When(@"I perform an operation that might fail")]
public void PerformOperation()
{
    try
    {
        // Perform operation
        DoSomething();
    }
    catch (Exception ex)
    {
        _scenarioContext["LastException"] = ex;
        // Don't re-throw; let Then step verify
    }
}

[Then(@"I should have caught an exception of type ""([^""]*)""")]
public void VerifyException(string exceptionType)
{
    var exception = _scenarioContext.Get<Exception>("LastException");
    Assert.IsNotNull(exception, "No exception was caught");
    Assert.AreEqual(exceptionType, exception.GetType().Name);
}
```

### Tip 5: Running Specific Tests by Tags

```bash
# Run only smoke tests
dotnet test --filter "Category=smoke"

# Run tests with multiple tags (AND logic)
dotnet test --filter "Category=smoke&Category=critical"

# Run excluding tests with certain tags
dotnet test --filter "Category!=slow"

# Using environment configuration
dotnet test -- TestRunParameters:Parameter(name="tags", value="@smoke")
```

---

## Resources

- [SpecFlow Official Documentation](https://specflow.org/documentation/)
- [Cucumber Gherkin Reference](https://cucumber.io/docs/gherkin/)
- [C# Automation Best Practices](https://docs.microsoft.com/en-us/dotnet/)
- [BDD Principles](https://cucumber.io/docs/bdd/)
- [SpecFlow GitHub Repository](https://github.com/SpecFlowOSS/SpecFlow)
- [Selenium WebDriver Documentation](https://www.selenium.dev/documentation/)

---

## Best Practices Checklist

- [ ] Feature files use business language, not technical implementation
- [ ] Each scenario has a single, clear behavior to test
- [ ] Step definitions are DRY (Don't Repeat Yourself)
- [ ] Tests are independent and can run in any order
- [ ] Proper use of hooks for setup and teardown
- [ ] Test data is not hardcoded in step definitions
- [ ] Meaningful assertion messages for debugging
- [ ] Tags are used consistently for test categorization
- [ ] All tests pass consistently (no flaky tests)
- [ ] Code follows C# naming conventions and style guidelines

---

## Contributing

Contributions are welcome! Please:
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

---

## Support

For questions or issues:
- Review the relevant section in the repository
- Check [SpecFlow documentation](https://specflow.org/documentation/)
- Refer to inline code comments and examples
- Review the [Cucumber BDD guide](https://cucumber.io/docs/bdd/)

---

## License

This project is open source and available for educational purposes.

---

**Happy Testing! 🚀**

*Last Updated: 2026-05-30*
*Framework: SpecFlow for .NET*
*Languages: C# & Gherkin*