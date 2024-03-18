# Tendable.com Automated Testing Project

This project contains automated tests for evaluating various elements on the Tendable.com website.

## Setup Instructions

1. **Clone Repository**: Clone this repository to your local machine.

2. **Install Dependencies**: Ensure you have Maven installed.

   
## Testing Strategy

### Page Classes
- Page classes encapsulate the behavior and elements of specific web pages.
- Each page class represents a distinct page on the Tendable.com website (e.g., HomePage, ContactUsPage).

### Flow Classes
- Flow classes define the high-level actions or user flows within the application.
- They utilize page classes to interact with the web pages and perform operations.

### Test Classes
- Test classes contain individual test cases implemented using TestNG.
- Each test class focuses on specific test scenarios related to the objectives outlined for the Tendable.com website.

## Test Objectives
1. Confirm accessibility of top-level menus.
2. Verify presence and activity of "Request a Demo" button on top-level menu pages.
3. Navigate to the "Contact Us" section, choose "Marketing", and complete the form—excluding the "Message" field. Verify the appearance of the error message upon submission.
4. Generate a bug report if the error message is not displayed when the "Message" field is empty.
## How to Run Tests

To run the automated tests for the Tendable.com website, follow these steps:

1. **Clone Repository**: Clone the Git repository containing the test project to your local machine.

2. **Install Dependencies**: Ensure you have Maven installed on your machine. Navigate to the project directory in your terminal or command prompt and run the following Maven command to install dependencies:

3. **Set Up WebDriver**: Download the appropriate WebDriver executable for your browser (e.g., ChromeDriver for Google Chrome) and ensure it's available in your system PATH or specify its location in the test configuration.

4. **Run Tests**: Execute the following Maven command to run the tests:


This command will trigger the execution of your TestNG tests. Maven will automatically look for test classes in the default directory structure (`src/test/java`) and execute them.

Additionally, you can use specific Maven goals to control the test execution:
- `mvn clean test`: This command will clean the project, compile the source code, run tests, and generate test reports.
- `mvn test -Dtest=TestClassName`: This command will run only the test class specified by `TestClassName`.
- `mvn test -Dtest=TestClassName#testMethodName`: This command will run only the specific test method (`testMethodName`) within the specified test class (`TestClassName`).

Ensure that your project is properly configured with TestNG dependencies and that your test classes are correctly annotated with `@Test` annotations. Additionally, make sure your WebDriver setup is correctly configured to interact with the Tendable.com website.

By running the tests with Maven commands, you can easily integrate test execution into your CI/CD pipelines or automate test runs as part of your development workflow.

## using testNG 
Right click on Project then click on RunAs TestNg
## Reporting Bugs
If any test fails to meet the specified criteria, a bug report should be generated. The bug report should include details such as steps to reproduce the issue, expected vs. actual behavior, and relevant screenshots or logs.

## Author
Sachin Khade


