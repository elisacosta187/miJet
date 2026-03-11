# Test Plan: Account Information (Identity)

**URL**: [https://www.mijet.eu/gb/identity](https://www.mijet.eu/gb/identity)

## Form Overview

The Identity form on miJet is a streamlined version of the standard PrestaShop personal information form, focusing on essential account credentials and privacy consents.

## Test Cases

| ID | Title | Description | Expected Result |
| :--- | :--- | :--- | :--- |
| AI-01 | Email Field Display | Verify the email field is pre-filled with the current user's email. | Field contains the correct email and is editable. |
| AI-02 | Password Visibility Toggle | Enter text in the password field and click the "Show" button. | Password characters become visible; button text changes to "Hide". |
| AI-03 | Password Length Validation | Enter a password with <6 or >12 characters and click "Save". | System prevents submission and shows a validation error. |
| AI-04 | Mandatory Privacy Checkbox | Try to save changes without checking "Customer data privacy". | Form prevents submission and highlights the checkbox as required. |
| AI-05 | Newsletter Subscription | Toggle the "Sign up for our newsletter" checkbox and save. | Preference is saved correctly (verified by revisiting the page). |
| AI-06 | Successful Information Update | Update email (to a valid new one) and enter current password, then save. | Success message "Information successfully updated" is displayed. |
| AI-07 | Invalid Email Format | Enter an incorrectly formatted email (e.g., "test@com") and save. | Field-level validation error appears. |
| AI-08 | Current Password Required | Attempt to change the email without providing the current password. | System requires the password to authorize the change. |
| AI-09 | Language Switch | Change language using the selector. | Labels and system messages translate to the selected language. |

## Notes on Missing Fields
During exploration, standard fields such as **First Name**, **Last Name**, **Social Title**, and **Birthdate** were not visible on this form. Testing should confirm if these are intentionally hidden or if they appear under specific account conditions.
