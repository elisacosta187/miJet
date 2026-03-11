# Test Plan: Account Addresses

**URL**: [https://www.mijet.eu/gb/addresses](https://www.mijet.eu/gb/addresses)

## Form Overview

The Addresses section on miJet allows users to manage multiple shipping and billing addresses. The form is tailored to have several mandatory fields, including Company and VAT number, which suggests a B2B focus.

## Test Cases

| ID | Title | Description | Expected Result |
| :--- | :--- | :--- | :--- |
| AD-01 | Addresses List View | Navigate to the "Addresses" page. | Page displays "Your Invoice Address", "Shipping Addresses", and "Other Addresses" if they exist. |
| AD-02 | Create New Address Form | Click on "+ Create new address". | Form opens with all expected fields (First name, Last name, Company, VAT, etc.). |
| AD-03 | Mandatory Fields Validation | Attempt to "Save" an empty form. | System prevents submission and highlights all mandatory fields (marked with *). |
| AD-04 | VAT Number Validation | Enter an invalid VAT number format and try to save. | System displays a validation error for the VAT number. |
| AD-05 | Successful Address Creation | Fill in all mandatory fields with valid data and click "Save". | Success message "Address successfully added!" appears; address is listed in the addresses page. |
| AD-06 | Address Update | Click "Update" on an existing address, change a field (e.g., Phone), and save. | Changes are saved and reflected in the address list. |
| AD-07 | Address Deletion | Click "Delete" on an address and confirm. | Address is removed from the account; success message is displayed. |
| AD-08 | Country Dropdown | Select a different country (e.g., Italy vs. UK). | Form may update field requirements (e.g., Postal Code format) based on the country selection. |
| AD-09 | Optional Fields | Fill in mandatory fields but leave "Address Complement" and "Phone" empty. | Address is successfully saved as these fields are optional. |
| AD-10 | Language Switch | Change language using the selector. | Form labels, button text, and messages translate correctly. |

## Bugs

### AS-BUG-01 - Low:

Account page > Address Management > If I have more than one "Other addresses", I see them with no padding.
