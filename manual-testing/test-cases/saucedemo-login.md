# Saucedemo — Login Test Cases

**Date:** 2026-06-02
**Tester:** Gustas
**Browser / OS:** Chrome 148.0.7778.181 / macOS Tahoe 26.5
**URL:** https://www.saucedemo.com

---

## TC-LOGIN-001 — Successful login with valid standard user credentials

| Field               | Value                                                                                                                                 |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| **Test Case ID**    | TC-LOGIN-001                                                                                                                          |
| **Description**     | Verify successful login with valid standard user credentials                                                                          |
| **Preconditions**   | Browser is open, user is on saucedemo.com login page                                                                                  |
| **Test Data**       | Username: `standard_user` · Password: `secret_sauce`                                                                                  |
| **Test Steps**      | 1. Enter username into the Username field · 2. Enter password into the Password field · 3. Click the "Login" button                   |
| **Expected Result** | User is redirected to `inventory.html`; page displays product listing with at least 6 items; hamburger menu is accessible in top-left |
| **Postconditions**  | User session is active; cart icon shows "0" items                                                                                     |

---

## TC-LOGIN-002 — Error handling with invalid username

| Field               | Value                                                                                                                                |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **Test Case ID**    | TC-LOGIN-002                                                                                                                         |
| **Description**     | Verify that login is denied and an error message is displayed when invalid username is entered                                       |
| **Preconditions**   | Browser is open, user is on saucedemo.com login page                                                                                 |
| **Test Data**       | Username: `standard_userfalse` · Password: `secret_sauce`                                                                            |
| **Test Steps**      | 1. Enter username into the Username field · 2. Enter password into the Password field · 3. Click the "Login" button                  |
| **Expected Result** | User is blocked from logging in; error message is shown: "Epic sadface: Username and password do not match any user in this service" |
| **Postconditions**  | User stays in login page; error message is visible                                                                                   |

---

## TC-LOGIN-003 — Error handling with invalid user credentials

| Field               | Value                                                                                                                                |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **Test Case ID**    | TC-LOGIN-003                                                                                                                         |
| **Description**     | Verify that login is denied and an error message is displayed when invalid credentials are entered                                   |
| **Preconditions**   | Browser is open, user is on saucedemo.com login page                                                                                 |
| **Test Data**       | Username: `standard_userfalse` · Password: `secret_saucefalse`                                                                       |
| **Test Steps**      | 1. Enter username into the Username field · 2. Enter password into the Password field · 3. Click the "Login" button                  |
| **Expected Result** | User is blocked from logging in; error message is shown: "Epic sadface: Username and password do not match any user in this service" |
| **Postconditions**  | User stays in login page; error message is visible                                                                                   |

---

## TC-LOGIN-004 — Log in is blocked for the locked out user

| Field               | Value                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **Test Case ID**    | TC-LOGIN-004                                                                                                        |
| **Description**     | Verify that log in is blocked with locked out user credentials                                                      |
| **Preconditions**   | Browser is open, user is on saucedemo.com login page                                                                |
| **Test Data**       | Username: `locked_out_user` · Password: `secret_sauce`                                                              |
| **Test Steps**      | 1. Enter username into the Username field · 2. Enter password into the Password field · 3. Click the "Login" button |
| **Expected Result** | User is blocked from logging in; error message is shown: "Epic sadface: Sorry, this user has been locked out."      |
| **Postconditions**  | User stays in login page; error message is visible                                                                  |

---

## TC-LOGIN-005 — Empty password field

| Field               | Value                                                                                                   |
| ------------------- | ------------------------------------------------------------------------------------------------------- |
| **Test Case ID**    | TC-LOGIN-005                                                                                            |
| **Description**     | Verify that login is denied and an error message is displayed when password input is left empty         |
| **Preconditions**   | Browser is open, user is on saucedemo.com login page                                                    |
| **Test Data**       | Username: `standard_user` · Password: [empty]                                                           |
| **Test Steps**      | 1. Enter username into the Username field · 2. Leave password field empty · 3. Click the "Login" button |
| **Expected Result** | User is blocked from logging in; error message is shown: "Epic sadface: Password is required"           |
| **Postconditions**  | User stays in login page; error message is visible                                                      |

---
