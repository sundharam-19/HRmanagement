Automated Testing of HR Management Web Application

Project Title :

Automated Testing of the Web Application using Python Selenium Framework

Application Under Test :

https://opensource-demo.orangehrmlive.com

---

Project Objective :

The objective of this project is to automate the testing of the OrangeHRM web application by simulating real-world user actions and validating core functionalities.

The framework validates :

1.Login functionality

2.Menu accessibility

3.User management

4.Forgot password functionality

5.Leave assignment

6.Claim request

7.My Info section validation

8.Cross-browser compatible automation execution

9.Reporting using Allure Reports

---

Technology Stack                                           Technology Purpose

Python 3.11                                                Programming Language
Selenium WebDriver                                         Browser Automation
Pytest Test                                                Execution Framework
Allure Report                                              Test Reporting
ChromeDriver                                               Browser Driver
CSV                                                        Test Data Management
Page Object Model (POM)                                    Framework Design Pattern

---

Project Structure :

HRmanagement/
│
├── tests/
│ ├── test_login.py
│ ├── test_home_page.py
│ ├── test_login_fields.py
│ ├── test_menu_validation.py
│ ├── test_create_user.py
│ ├── test_search_user.py
│ ├── test_assign_leave.py
│ ├── test_claim_request.py
│ ├── test_myinfo_menu.py
│ └── test_forgot_password.py
│
├── pages/
│ ├── login_page.py
│ └── dashboard_page.py
│
├── reports/
├── allure-results/
├── allure-report/
├── login_data.csv
├── csv_reader.py
├── conftest.py
├── config.py
├── pytest.ini
├── requirements.txt
└── README.md

---

Framework Features :

1.Page Object Model (POM) architecture

2.Data-driven testing using CSV

3.Explicit waits for synchronization

4.Reusable test components

5.Browser setup using Pytest fixtures

6.Allure reporting integration

7.Modular test design

8.Cross-browser compatible structure

9.Exception handling and validations

---

Test Scenarios Covered :

Test Case 1 - Login Validation :

Validate login functionality using multiple credentials from CSV file.

Validations

Valid login

Invalid login

Error message validation

Logout validation

---

Test Case 2 - Home URL Validation :

Verify that the OrangeHRM home page loads successfully.

---

Test Case 3 - Login Fields Validation :

Verify visibility and accessibility of:

Username field

Password field

Login button

---

Test Case 4 - Main Menu Validation :

Validate visibility and clickability of:

Admin

PIM

Leave

Time

Recruitment

My Info

Performance

Dashboard

---

Test Case 5 - Create User Validation :

Validate Admin page accessibility and user management functionality.

---

Test Case 6 - User Search Validation :

Validate Admin module accessibility and user search functionality.

---

Test Case 7 - Forgot Password Validation :

Validate Forgot Password link functionality and password reset page.

---

Test Case 8 - My Info Menu Validation :

Validate My Info module accessibility.

---

Test Case 9 - Assign Leave Validation :

Validate Leave module accessibility and leave assignment workflow.

---

Test Case 10 - Claim Request Validation :

Validate dashboard accessibility and claim request workflow.

---

Prerequisites :

Before running the project ensure the following are installed :

1.Python 3.11

2.Google Chrome Browser

3.ChromeDriver

4.Java (for Allure)

5.Allure Report

6.PyCharm or VS Code

---

Python Package Installation :

Install required packages :

pip install selenium
pip install pytest
pip install pytest-html
pip install allure-pytest

OR

pip install -r requirements.txt

---

How to Run Tests :

Run All Tests :

pytest -v

---

Run Specific Test :

pytest test_login.py -v

---

Generate Allure Report :

Step 1 - Execute Tests :

pytest -v --alluredir=allure-results

---

Step 2 - Generate Report :

allure generate allure-results -o allure-report --clean

---

Step 3 - Open Report :

allure open allure-report

OR

allure serve allure-results

---

Sample Test Data :

username,password,expected
Admin,admin123,valid
Admin,wrongpass,invalid
wronguser,admin123,invalid

---

Design Pattern Used :

Page Object Model (POM)

The framework uses the Page Object Model design pattern to improve :

1.Code reusability

2.Readability

3.Maintainability

4.Scalability

---

Synchronization Strategy :

Explicit waits are implemented throughout the framework using :

WebDriverWait(driver, 20)

This ensures stable execution and avoids synchronization failures.

---

Reporting :

The framework supports :

1.Pytest Console Report

2.Allure Advanced HTML Report

----

Allure reports include :

1.Passed/Failed Tests

2.Execution Timeline

3.Graphs

4.Test Suites

5.Test Duration

6.Execution History

---

Exception Handling :

The framework includes :

1.Selenium exception handling

2.Explicit waits

3.Validation assertions

4.Stable XPath handling using normalize-space()

---

Best Practices Followed :

1.Clean code structure

2.Modular reusable methods

3.Proper naming conventions

4.Explicit waits

5.Page Object Model

6.Data-driven testing

7.Centralized configuration

8.Reusable fixtures

---

Conclusion

This project demonstrates a complete real-time Selenium automation framework using Python, Pytest, Page Object Model, Data-Driven Testing, and Allure Reporting.

The framework is scalable, maintainable, and suitable for enterprise-level web automation testing.
