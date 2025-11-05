# Simplify Money QA Automation

Automation scripts for testing the **Simplify Money Chatbot** using **Appium Java** and **TestNG**.  
This project validates core chatbot functionality, UI elements, and user input handling on Android devices.

---

## **Project Overview**
This repository contains automation scripts that cover the following test scenarios:

| Test Case ID | Feature | Scenario |
|-------------|--------|---------|
| TC01 | Chatbot | Send basic question |
| TC02 | Chatbot | Suggestion chip click |
| TC03 | Chatbot | Empty input |
| TC04 | Chatbot | Multiple questions |
| TC05 | Chatbot | Buttons existence |

**Purpose:**  
- Verify chatbot responses and interactions  
- Detect functional bugs  
- Provide logs, screenshots, and suggestions for QA improvements  

---

## **Prerequisites**
Before running the tests, ensure you have the following installed:

- **Java 17** or higher  
- **Maven** (for dependency management)  
- **Android Studio** (for emulator or device setup)  
- **Appium Server** (v2.x recommended)  
- **Android Device / Emulator** with Developer Options enabled  

---

## **Installation**
1. Clone the repository:
```bash
git clone <your-github-repo-link>
cd SimplifyMoney-QA-Automation
```

- Install dependencies using Maven:

mvn clean install

- Ensure Appium server is running and your Android device/emulator is connected.

Running Tests

You can run the tests using IntelliJ IDEA or command line:

Using IntelliJ:

Open testing.xml (TestNG suite)

Right-click → Run

Using Command Line:

mvn test -DsuiteXmlFile=testing.xml

Project Structure
SimplifyMoney-QA-Automation/
``` bash
├── src/
│ ├── main/
│ │ └── java/ # Page objects and helper classes
│ └── test/
│ └── java/ # Test scripts
├── pom.xml # Maven dependencies
├── testing.xml # TestNG suite
├── target/ # Test reports and screenshots
│ └── screenshots/ # Captured screenshots for failed tests
└── README.md # Project documentation
```
Test Execution Reports
- All test cases are executed via TestNG

Screenshots are captured for failed scenarios (target/screenshots)
- Logs and console output provide detailed steps of execution

Known Issues / Bugs
- Input field visibility can fail under rapid message entry.

- SLF4J warnings may appear in console (non-critical).
