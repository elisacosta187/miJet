# Test Plan: Order History

**URL**: [https://www.mijet.eu/gb/order-history](https://www.mijet.eu/gb/order-history)

## Overview

The Order History section provides users with a comprehensive list of their past purchases, including order status tracking and the ability to view detailed invoices or reorder items.

## Test Cases

### 1. Empty State
| ID | Title | Description | Expected Result |
| :--- | :--- | :--- | :--- |
| OH-01 | Empty History Message | Access history with a new account (no orders). | Message "You have not yet placed orders" is displayed with a placeholder graphic. |
| OH-02 | Shop CTA | Click the "Shop MiJET®" or "Buy MiJET®" button from the empty state. | User is redirected to the product category page. |
| OH-03 | Support Link | Click the "Contact support" link. | User is redirected to the Contact page. |

### 2. Order List (Populated)
| ID | Title | Description | Expected Result |
| :--- | :--- | :--- | :--- |
| OH-04 | Order List Display | Access history with an account that has previous orders. | List displays Reference, Date, Total Price, Payment Method, and Status. |
| OH-05 | Sorting/Filtering | Attempt to sort or filter the order list (if available). | List updates to reflect the selected criteria. |
| OH-06 | Reorder Functionality | Click the "Reorder" link next to a previous order. | Items from that order are added to the cart; user is redirected to the cart page. |
| OH-07 | Order Details Access | Click "Details" for a specific order. | User is taken to the Order Detail page (`/gb/order-detail`). |

### 3. Order Details View
| ID | Title | Description | Expected Result |
| :--- | :--- | :--- | :--- |
| OH-08 | Order Summary | Verify details: Reference, Date, and Status History. | Information matches the actual order data. |
| OH-09 | Address Verification | Verify Shipping and Invoice addresses in the details view. | Addresses match those provided during checkout. |
| OH-10 | Product List & Totals | Check the list of items, unit prices, and final total. | Calculations are accurate and items are correctly listed. |
| OH-11 | PDF Invoice | Click the "Download your invoice" link (if status allows). | A PDF version of the invoice is downloaded. |
| OH-12 | Language Switch | Change language using the selector. | List headers, order statuses, and detail labels translate correctly. |
