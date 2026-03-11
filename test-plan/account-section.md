# Test Plan: Account Section

**URL**: [https://www.mijet.eu/gb/my-account](https://www.mijet.eu/gb/my-account)

## Test Cases

| ID | Title | Description | Expected Result |
| :--- | :--- | :--- | :--- |
| AS-01 | Account Page Access | Navigate to the "My Account" page while logged in. | Page loads correctly with all information tiles (Information, Addresses, etc.). |
| AS-02 | Personal Information Update | Click on "Information" and update a field (e.g., telephone). | Change is saved and reflected in the user profile. |
| AS-03 | Address Management | Click on "Addresses" and add a new delivery address. | New address is saved and appears in the list of addresses. |
| AS-04 | Order History | Click on "Order History" and view a past order. | Order details (items, date, status, total) are correctly displayed (or empty state if none exist). |
| AS-05 | Credit Notes | Click on "Credit Notes" to view refunds/credits. | Shows a list of credit slips (or empty state if none exist). |
| AS-06 | Password Change | Attempt to change the account password from the Information section. | Password is updated correctly after providing the current one. |
| AS-07 | Logout | Click the "Disconnect" button. | User is logged out and redirected to the home page or login page. |
| AS-08 | Authentication Guard | Attempt to access `/gb/my-account` after logging out. | User is redirected to the login page. |
| AS-09 | Language Switch | Change language using the selector. | Account tile titles and descriptions translate correctly. |
