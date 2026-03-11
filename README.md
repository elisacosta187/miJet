# miJet E-commerce Test Plan

This directory contains a comprehensive set of test plans for the [miJet](https://www.mijet.eu/gb/) e-commerce website. These plans are designed to ensure the quality and reliability of the user experience across all major pages and functionalities.

## Test Strategy

The testing strategy focuses on:
- **Functional Testing**: Verifying that all features work as expected (navigation, language switch, cart, checkout).
- **UI/UX Testing**: Ensuring the interface is responsive, elements are correctly displayed, and the experience is intuitive.
- **Form Validation**: Checking that contact and checkout forms handle inputs correctly.
- **Ecommerce Flow**: End-to-end testing of the purchasing process. **This one is TBC as there is only prod environment and I see some orders have been placed already**

## Test Plans

1. [Home Page](/test-plan/home-page.md): Landing page, global navigation, and hero sections.
2. [Category Page](/test-plan/category-page.md): Product listings and filtering.
3. [Product Page](/test-plan/product-page.md): Detailed product information and interactions.
4. [Contact & Company](/test-plan/contact-page.md): Contact forms and informational pages.
5. [Cart & Checkout](/test-plan/cart-checkout.md): Shopping basket management and the multi-step order process.
6. [Account Section](/test-plan/account-section.md): User profile overview and history management.
7. [Account Information](/test-plan/account-info.md): Detailed personal data, password, and privacy settings.
8. [Account Addresses](/test-plan/addresses.md): Detailed management of shipping and billing addresses.
9. [Order History](/test-plan/order-history.md): Detailed viewing of previous orders, statuses, and reordering.
10. [Credit Notes](/test-plan/credit-notes.md): Detailed viewing and downloading of credit slips.
11. [Guest Order Tracking](/test-plan/guest-tracking.md): Tracking orders as a guest user using order reference and email.
12. [Account Registration](/test-plan/registration.md): Creating a new user account and managing privacy consents.

## Tools Recommended

- **Playwright**: For automated end-to-end testing.
- **Manual QA**: For visual verification and usability edge cases.
