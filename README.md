![SwoopLogo](./SwoopLogo.png)
# Automated Testing for Swoop.ge

This repository contains an automated test script for performing a series of actions on the [Swoop.ge](https://swoop.ge) website using Selenium and Java. The test script is designed to automate a series of user interactions and validations, ensuring that the website functions correctly.

## Prerequisites

Before running the automated test, make sure you have the following prerequisites installed on your system:

- [Java Development Kit (JDK)](https://www.oracle.com/java/technologies/javase-downloads.html): Java 8 or later.
- [IntelliJ IDEA](https://www.jetbrains.com/idea/): A Java IDE (Integrated Development Environment).
- [Chrome WebDriver](https://sites.google.com/a/chromium.org/chromedriver/downloads): Download the Chrome WebDriver executable and ensure it's in your system's PATH.
- [Edge WebDriver](https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/): Download the Edge WebDriver executable and ensure it's in your system's PATH.

## Setup

1. Clone this repository to your local machine:

   ```bash
   git https://github.com/Skhila/Project-SwoopTest.git
   ```

2. Open the project in IntelliJ IDEA.

3. Configure the project to use the appropriate JDK and dependencies.

## Running the Test

To run the automated test, follow these steps:

1. Open the `testNG.xml` file in IntelliJ IDEA.

2. Right-click within the file and select "Run 'SwoopAutomationTest'".

3. The test will open a Chrome browser, navigate to the [Swoop.ge](https://swoop.ge) website, and perform a series of actions as described in the task.

4. The test will check for valid data, click buttons, choose vacant seat, register and verify the correctness of movie information and error messages.

5. The test results will be displayed in the IntelliJ IDEA console.

## Test Flow

The automated test follows the specified task flow:

1. Opens the Chrome browser.
2. Navigates to the [Swoop.ge](https://swoop.ge) website.
3. Goes to the 'კინო' section.
4. Selects the first movie in the returned list and clicks on the ‘ყიდვა’ button.
5. Scrolls vertically and horizontally to choose ‘კავეა ისთ ფოინთი’ options.
6. Checks that only ‘კავეა ისთ ფოინთი’ options are returned.
7. Clicks on the last date and then clicks on the last option.
8. Checks in the opened popup that movie name, cinema, and datetime are valid.
9. Chooses any vacant place.
10. Registers for a new account.
11. Fills all fields with valid data except for email.
12. Checks that the error message ‘მეილის ფორმატი არასწორია!' appears.

## Test Results

The test script will provide detailed output in the console, including whether each step of the test passed or failed. It will also display any error messages encountered during the test.

## Notes

- This automated test is intended for demonstration and educational purposes.
- Ensure that your environment is set up correctly, including the JDK and Chrome WebDriver.
- The test may need adjustments if the structure or behavior of the [Swoop.ge](https://swoop.ge) website changes.

Happy testing!