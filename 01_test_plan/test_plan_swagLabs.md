# Test Plan - Swag Labs

## 1. Introduction
This document details the Test Plan for the Swag Labs demo website (https://www.saucedemo.com/). The primary objective is to validate the application's functionality and usability, and to identify possible defects before a hypothetical product release.


## 2. Scope Test
### 2.1. Functionalities to test
* **User Management :**
    * Login (authentication with valid/invalid credentials).
    * Logout.
* **Product Navigate and Visualization:**
    * Inventory page loading
    * Viewing all products with details (name, description, price, image).
    * Product sorting(name [A-Z] OR [Z-A], price [LOW-HIGH] OR [HIGH-LOW]).
    * Navigate to product detail page and back. 
* **Shopping Cart:**
    * Adding products to the cart.
    * Removing products from the cart.
    * Car counter updates.
    * Viweing items in the cart.
* **Checkout Process:**
    * Starting checkout process.
    * Entering customer information(rirst name, last name, postal code).
    * Order overview (items, prices, taxes, total).
    * Complete the purchase.
    * Confirmation messages.
* **Main Menu:**
    * Navegagion to "All Items", "About", "Logout".

### 2.2. Functionalities Out of Scope
* Integration testing with external systems (real payment gateways).
* Load/Stress testing(beyond basic manual observation).
* Advanced Security Testing (SQL injection, XSS, DDoS, Phishing)
* Logical validation of tax or discount.

## 3. Test Strategy
The following test types will be executed: 
* **Functional Testting:** To ensure each feature behaves according to requirements.
* **Usability Testing:** To verify that the interfaz is intuitive and user-friendly.
* **Exploratory Testing:** Exploring the application without predefined test cases, using their experience and intuition to discover defects, usability issues, or unexpected behaviors. This approach helps identify issues that may not be covered by scripted tests.


## 4. Test Environment
* **Application URL:** https://www.saucedemo.com/
* **Test Credentials:**
    * **Standard User:** `standard_user` : `secret_sauce`
    * **Problem User (for exploratory tests):** `problem_user` : `secret_sauce`
    * **Performance GLitch User (for exploratory tests):** `performance_glitch_user` / `secret_sauce`
* **Browsers:**
    * Mozilla Firefox(Mozilla Firefox 135.0)
    * Google Chrome (Chrome 137)
    * Brave (Brave v1.79.119)
* **Operating Systems:** Windows 10, Linux/Ubuntu (Ubuntu 24.04.2 LTS)

## 5. Entry and Exit Criteria
### 5.1. Entry Criteria
* The test environment is set up and accessible.
* The Swag Labs application is deployed and functional at the specified URL.
* Test credentials are known and valid.
* The plan test and initial cases test have been reviewed and approved.

### 5.2. Exit Criteria
* At least 90% of high-priority and critical test cases have passed.
* All critical and major defects have been reported.
* No new critical defects have been found in the last 24 hours of testing.
* Exploratory test have been completed.

## 6. Roles and Responsabilities
* **QA Tester:** [Juan] (responsible for planning,design, executing tests, and reporting defects).

## 7. Deliverables
* Test Plan
* Test Cases (with execution resuts)
* Defect Reports
* Defect Evidence (screenshots/videos)

## 8. Tools
* Documentation: Markdown (`.md`), excel (`.xlsx`)
* Version Control: Git / GitHub
* Browsers (Chrome, Firefox, brave)
* Developer Tools  (F12) for basic debugging