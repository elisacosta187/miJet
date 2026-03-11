# Test Plan: Account Registration

**URL**: [https://www.mijet.eu/gb/registration](https://www.mijet.eu/gb/registration)

## Overview

The Account Registration page allows new users to create an account by providing their personal details and consenting to data privacy policies.

## Test Cases

| ID | Title | Description | Expected Result |
| :--- | :--- | :--- | :--- |
| RE-01 | Page Access | Navigate to the registration page. | Page loads correctly with all form fields visible. |
| RE-02 | Form Validation (Empty) | Click "Save" without filling any fields. | Mandatory fields (First Name, Last Name, Email, Password, Privacy) are highlighted as required. |
| RE-03 | Fields Format Validation | Enter invalid email format or password < 6 characters. | System shows validation errors for the specific fields. |
| RE-04 | Password Visibility | Enter text in password field and click "Show". | Password becomes visible; toggle text changes to "Hide". |
| RE-05 | Mandatory Privacy Checkbox | Fill form correctly but leave Privacy checkbox unchecked. | Form prevents submission and highlights the privacy requirement. |
| RE-06 | Login Link | Click the "Log in here!" link. | User is redirected to the Login page. |
| RE-07 | Newsletter Subscription | Toggle the "Sign up for our newsletter" checkbox. | Checkbox state changes correctly; preference is recorded upon submission (theoretical). |
| RE-08 | Language Switch | Change language using the selector. | Form labels, mandatory markers, and privacy section translate correctly. |

## Notes
- **Mandatory Fields**: First Name, Last Name, Email, Password, and Customer Data Privacy are required.
- **Password Requirement**: Between 6 and 12 characters.
