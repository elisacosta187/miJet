# Test Plan: Cart & Checkout

**Cart URL**: [https://www.mijet.eu/gb/cart?action=show](https://www.mijet.eu/gb/cart?action=show)
**Checkout URL**: [https://www.mijet.eu/gb/order](https://www.mijet.eu/gb/order)

## Test Cases

| ID | Title | Description | Expected Result |
| :--- | :--- | :--- | :--- |
| CH-01 | Cart Summary | Verify items, quantities, and prices in the cart. | All data is consistent with what was added. |
| CH-02 | Quantity Updates | Change quantity of an item within the cart. | Subtotal and total amounts are updated in real-time. |
| CH-03 | Item Removal | Click the trash icon to remove an item. | Item is removed, and the cart summary updates correctly. |
| CH-04 | Multi-step Checkout | Navigate through the 4 steps (Personal Info, Addresses, Shipping, Payment). | Progress indicator reflects current step; data is preserved between steps. |
| CH-05 | Checkout Form Validation | Leave mandatory fields empty in the checkout flow. | Form prevents proceeding and shows validation errors. |
| CH-06 | Guest vs. Registered | Attempt checkout as a guest and with an existing account. | Both flows function correctly (login vs. account creation). |
| CH-07 | Order Summary Sidebar | Check the order summary in the sidebar during checkout. | Displays accurate totals and item counts at every step. |
| CH-08 | Language Switch | Change language using the selector during checkout. | Checkout steps, labels, and summaries translate correctly. |

## Bugs:

### CH-BUG-01 - High:

Cart page > when I update quantity in the cart, the total amount is not updated, I have to refresh the page to see the updated total amount.

### CH-BUG-02 - Medium:

Checkout page > addresses > if I only have one shipping address, this is not automatically selected, if I continue without selecting it, I see the page refreshes but I do not see any errors. We can either pre-select the only available address OR we can show an error message to the user when they attempt to continue without selecting a shipping address.
