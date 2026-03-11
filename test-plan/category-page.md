# Test Plan: Category Page

**Example URL**: [https://www.mijet.eu/gb/6-accessories](https://www.mijet.eu/gb/6-accessories)

## Test Cases

| ID | Title | Description | Expected Result |
| :--- | :--- | :--- | :--- |
| CP-01 | Product Grid Display | Verify all products show name, price, and image. | All elements are visible and correctly aligned. |
| CP-02 | Category Filters | Apply filters (e.g., Model ø20cm vs ø30cm). | Product list updates to show only matching items. |
| CP-03 | Quick "Add to Cart" | Click "Add to Cart" directly from the category grid. | Product is added to the cart, and a confirmation/cart update occurs. |
| CP-04 | Product Navigation | Click on a product name or image. | User is redirected to the correct Product Detail Page (PDP). |
| CP-05 | Breadcrumbs | Click on breadcrumb links (e.g., Home > Accessories). | Navigation follows the hierarchy correctly. |
| CP-06 | Language Switch | Change language using the selector. | Category name, filters, and product labels translate correctly. |

## Bugs:

### CP-BUG-01 - Low:

Category page > when I switch to Italian or French, `Low noise nozzle` is not translated (other products are).

### CP-BUG-02 - Low:

Category page > product cards > no spacing between quantity field and add to cart button (both on mobile and desktop), is that expected?

### CP-BUG-03 - Low:

Category page > header > breadcrumb `Accessories and Spare Parts` and category description `Discover all MiJET® accessories to optimize your system.` are not translated to French.
