# Test Plan: Product Page

**Example URL**: [https://www.mijet.eu/gb/filtri/21-filtro-di-ricambio-per-unita-mijet-20-cm.html](https://www.mijet.eu/gb/filtri/21-filtro-di-ricambio-per-unita-mijet-20-cm.html)

## Test Cases

| ID | Title | Description | Expected Result |
| :--- | :--- | :--- | :--- |
| PP-01 | Product Images | Click on product image. | Seelcted image (if more than one available) is displayed as main image. |
| PP-02 | Version Selection | Select different product versions (if applicable). | Price and specifications update according to the selection. |
| PP-03 | Quantity Selector | Use +/- buttons or enter a quantity manually. | Quantity updates correctly, ensuring it's a positive integer. |
| PP-04 | "Add to Basket" | Click "Add to Basket" button. | Product is added, and a confirmation modal/notification appears. |
| PP-05 | Technical Specs | Verify the presence and accuracy of technical specifications. | Data matches the product being viewed. |
| PP-06 | Language Switch | Change language using the selector. | Page content (title, description, specs) translates correctly. |


## Bugs:

### PP-BUG-01 - Medium:

Product page > Details tab is empty on main product page (in all languages).


### PP-BUG-02 - Low:

Product page > Details tab is empty on some product pages or shown in wrong language (e.g. https://www.mijet.eu/fr/filtri/21-filtro-di-ricambio-per-unita-mijet-20-cm.html I see Italian details translation when French is selected, and empty detailss ection when English is selected).

## Notes
I see they're missing in prestashop, so it's just a reminder to add them.
