# Test Plan: Home Page

**URL**: [https://www.mijet.eu/gb/](https://www.mijet.eu/gb/)

## Test Cases

| ID | Title | Description | Expected Result |
| :--- | :--- | :--- | :--- |
| HP-01 | Global Navigation | Click on all main menu items (Find out more, Accessories, Contact us). | Each link directs to the correct URL and the page loads. |
| HP-02 | Logo Link | Click the MiJET logo from the home page and subpages. | The user is always redirected back to the home page. |
| HP-03 | Hero Section CTAs | Click "Buy MiJET" and "Discover how it works" buttons. | "Buy MiJET" goes to product, "Discover" scrolls to info section. |
| HP-04 | Language Selector | Change language using the selector (top right). | Content updates to the selected language (e.g., Italian, French). |
| HP-05 | 20CM/30CM tab | Click on the 20CM and 30CM tabs. | The content updates to show the selected tab. |
| HP-06 | Footer Links | Verify all social media and informational links in the footer. | Links open in new tabs or navigate correctly to info pages. |
| HP-07 | Responsive Layout | View the home page on mobile and desktop. | Layout adjusts correctly, menu transforms to hamburger on smaller screens. |


## Bugs:

### HP-BUG-01 - Medium:

Hero Section > Click "Buy MiJET" > I am taken to top of the page instead of product page https://www.mijet.eu/gb/blowing-stations/20-mijet.html.
I would also expect to land in product page with correct product model selected (if 20cm tab is selected, I expect to land in 20cm product page, if 30cm tab is selected, I expect to land in 30cm product page). But that is a nice to have.

### HP-BUG-02 - Medium:

Footer > Sign up > Privacy Policy link takes me to an error page: https://www.mijet.eu/gb/%1$.

### HP-BUG-03 - Low:

Footer > Sign up > after filling input with already registered email, I am taken to the top of the page, so I do not see error message "This email address is already registered." unless I scroll to the footer again.

### HP-BUG-04 - Low:

Footer > Sign up > after filling input with a new email, I am taken to the top of the page, so I do not see success message "You have successfully subscribed to this newsletter." unless I scroll to the footer again.

### HP-BUG-05 - Low:

Footer > Privacy Policy page (https://www.mijet.eu/gb/content/2-privacy-policy), Terms of Service page (https://www.mijet.eu/gb/content/3-terms-and-conditions) and Cookies Settings page (https://www.mijet.eu/gb/content/7-cookies-policy) are not really pleasant to see.

### HP-BUG-06 - Low:

Footer > Facebook link: https://www.facebook.com/cssflys.mijet takes to a not available content, not sure this is expected.

### HP-BUG-07 - Low:

Footer > accessories links > when I switch to Italian or French, `Low noise nozzle` is not translated (other products are).
