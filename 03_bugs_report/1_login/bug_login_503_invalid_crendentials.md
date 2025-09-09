# 🐞 Bug Report

**BUG ID:** BUG_LOGIN_WRONG_CODE

**Title:** The login function returns 503(Service Unavailable) for invalidate credentials

## 📌 Description
When attempting to log in with invalid credentials, the authentication "http://www.saucedemo.com" incorectly returns a HTTP 503 Service Unavailable status code instead of the expected code 401 Unauthorized or 403 Forbidden.

## 🖥️ Environment
- OS: Windows 10 Pro 64-bit  
- Browser: Google Chrome Versión 139.0.7258.155 (Build oficial) (64 bits)  
- Environment: QA / https://www.saucedemo.com/inventory.html 

## 🔎 Preconditions
- User is logged out of the application

## 📝 Steps to Reproduce
- Go to the Swag Lab page login https://www.saucedemo.com/inventory.html 
- Open your browser's Developer Tools (F12) and navigate to the "Network" tab.
- Enter an invalid username and password into the respective fields.
- Observe the network requet made for authentication in the developer tool.

## ✅ Expected Result
The login request should return an HTTP status code of 401 Unauthorized or 403 Forbidden.

## ❌ Actual Result
The login request returns an HTTP status code of 503 Service Unavailable.

## 📂 Evidence
![login_wrong_code](../../bug_images/login_code_status_503.png)

## 🎯 Severity / Priority
- **Severity:** High
- **Priority:** High



