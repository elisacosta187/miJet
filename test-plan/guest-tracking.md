# Test Plan: Guest Order Tracking

**URL**: [https://www.mijet.eu/gb/guest-tracking](https://www.mijet.eu/gb/guest-tracking)

## Overview

The Guest Order Tracking page allows users who placed an order without creating an account to check their order status using their order reference and the email address used during checkout.

## Test Cases

| ID | Title | Description | Expected Result |
| :--- | :--- | :--- | :--- |
| GT-01 | Page Access (Guest) | Access the URL as a non-authenticated user. | Page loads correctly with "Guest Order Tracking" title and form. |
| GT-02 | Redirect for Logged-in Users | Access the URL while logged into an account. | User is automatically redirected to the Order History page. |
| GT-03 | Form Validation (Empty Fields) | Leave fields empty and click "Send". | System indicates that fields are mandatory and prevents submission. |
| GT-04 | Invalid Data Validation | Enter a non-existent order reference or incorrect email. | An error message is displayed (e.g., "Order not found"). |
| GT-05 | Successful Order Tracking | Enter a valid order reference and matching email. | User is redirected to the Order Detail page for that specific order. |
| GT-06  | Unsuccessful Order Tracking | Enter a valid order reference and wrong email. | An error message is displayed (e.g., "Order not found, try again"). |
| GT-07 | Language Switch | Change language using the selector. | Form labels, instructions, and button text translate correctly. |

## Notes
- Authenticated users cannot access this page directly as they are expected to use the standard "Order History" section in their account.
- The order reference is typically a 9-character uppercase string (e.g., QIIXJXNUI).


## Bugs

### GT-BUG-01 - High:

Guest Order Tracking > page layout has to be revised.

### GT-BUG-02 - High:

Guest Order Tracking > If I enter a valid order reference and a valid email address I correctly land on tracking page but page is visibly broken.
