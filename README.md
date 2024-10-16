# Heliverse-script

This project is an automation testing suite for a Shopify e-commerce website, built using Selenium WebDriver, TestNG, and Java. It covers various test cases, including functional tests, login tests, UI tests, and form validation tests. The test suite generates detailed test reports using Allure for better test result visualization.

## Prerequisites

- Java Development Kit (JDK)- Make sure you have JDK 8 or later installed.
- Maven- To manage project dependencies.
- IDE - An integrated development environment like IntelliJ IDEA or Eclipse.
- Browser - Google Chrome 

## Setting Up the Environment

1. Clone the Repository
   - Clone this project to your local machine using:
     git clone https://github.com/Sowmiya2189/Heliverse-script.git
     
   - Navigate to the project directory:
   
     cd Heliverse-script
     

2. Import the Project into Your IDE
   - Open your IDE (Eclipse).
   - Import the project as a Maven project to automatically load the dependencies.

3. Install Required Dependencies
   - Open the `pom.xml` file in the project and ensure that all the dependencies listed below are added:
     ```xml
     <dependencies>
         <!-- Selenium WebDriver -->
         <dependency>
             <groupId>org.seleniumhq.selenium</groupId>
             <artifactId>selenium-java</artifactId>
             <version>4.4.0</version>
         </dependency>

         <!-- TestNG -->
         <dependency>
             <groupId>org.testng</groupId>
             <artifactId>testng</artifactId>
             <version>7.4.0</version>
         </dependency>

         <!-- WebDriverManager -->
         <dependency>
             <groupId>io.github.bonigarcia</groupId>
             <artifactId>webdrivermanager</artifactId>
             <version>5.1.0</version>
         </dependency>

         <!-- Allure Reporting -->
         <dependency>
             <groupId>io.qameta.allure</groupId>
             <artifactId>allure-testng</artifactId>
             <version>2.13.9</version>
         </dependency>
     </dependencies>
     ```
   - Maven will automatically download and install these dependencies.

 Executing the Tests

To run the test cases, follow these steps:

1. Open TestNG Test Suite
   - Right-click on the `testng.xml` file in your IDE and select the option to run the TestNG suite.

Generating Test Reports

This project uses Allure to generate detailed test reports. Follow these steps to generate the reports:

1. Install Allure
   - Download and install Allure from (https://docs.qameta.io/allure/).

2. Generate the Report
   - Run the following command to generate the Allure test report:
     ```bash
     mvn allure:report
     ```

3. View the Report
   - To view the test report in your browser, use the command:
     ```bash
     mvn allure:serve
     ```
   - This command will start a local server and open the Allure report in your default web browser.

 Error Handling

- The test scripts include error handling that captures screenshots automatically whenever a test fails.


