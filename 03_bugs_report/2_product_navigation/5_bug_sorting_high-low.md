# 🐞 Bug Report

**BUG ID:** BUG_SORTED_HIGH_PRICE_005

**Title:** Products sorting by Price (high to low) does not work

## 📌 Descripcion
When the user select Price (high to low) option from the sort dropdown, the products are not ordened by price as expected.
This issue occurs with the users `problem_user` / `error_user`.

## 🖥️ Environment
- OS: Windows 10 Pro 64-bit  
- Browser: Google Chrome Versión 139.0.7258.155 (Build oficial) (64 bits)  
- Environment: QA / https://www.saucedemo.com/inventory.html 

## 🔎 Preconditions
- User logged in with:
    - Username: `problem_user` / Password: `secret_sauce`
    - Username: `error_user` / Password: `secret_sauce`
- User is on the inventory page (`/inventory.html`)

## 📝 Steps to Reproduce
1. Navigate to https://www.saucedemo.com/
2. Log in with any of the users mentioned in Preconditions.
3. Click 'Login' button.
4. Open the sort dropdown(top right).
5. Select Price (high to low).
6. Observe the product order by price.

## ✅ Expected Result
- Products should be ordered by price from high to low.

## ❌ Actual Result
- Products are not correctly ordered by price.

## 📂 Evidence
![Bug_sorted_low](../bug_images/bug_sorted_high_price.png)

## 🎯 Severity / Priority
- **Severity:** low (affects product presentation but app is still usable)  
- **Priority:** low  


## 🔗 Related Test Case
- [**TC_Product_Navigation_11**](../../02_test_cases/2_product_navigation/product_navigation2.png)
- [**TC_Product_Navigation_15**](../../02_test_cases/2_product_navigation/product_navigation2.png)

