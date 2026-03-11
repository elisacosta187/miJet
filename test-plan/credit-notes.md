# Test Plan: Credit Notes

**URL**: [https://www.mijet.eu/gb/credit-slip](https://www.mijet.eu/gb/credit-slip)

## Overview

The Credit Notes section displays all credit slips issued to the user, typically following order cancellations or refunds. Users can view the associated order reference and download the credit slip in PDF format.

## Test Cases

### 1. Empty State
| ID | Title | Description | Expected Result |
| :--- | :--- | :--- | :--- |
| CN-01 | Empty History Message | Access credit notes with a new account (no refunds). | Message "No credit slips received" is displayed with a placeholder graphic. |
| CN-02 | Return to My Orders | Click the "Return to my orders" button. | User is redirected to the Order History page. |

### 2. Credit Notes List (Populated)
| ID | Title | Description | Expected Result |
| :--- | :--- | :--- | :--- |
| CN-03 | Credit Notes Display | Access page with an account that has received credit slips. | List displays Credit Slip Number, Associated Order Reference, and Date. |
| CN-04 | PDF Download | Click on the PDF icon or "PDF" link for a credit slip. | A PDF file of the credit slip is downloaded correctly. |
| CN-05 | Order Reference Link | Click on the associated order reference. | User is redirected to the details page of that specific order. |
| CN-06 | Language Switch | Change language using the selector. | Table headers and informational messages translate correctly. |

## Notes on Generation
Credit slips are generated automatically by the system when:
1. An order is partially or fully canceled.
2. A return represents a value to be credited back to the customer.
3. A manual credit is issued by the administrator.
