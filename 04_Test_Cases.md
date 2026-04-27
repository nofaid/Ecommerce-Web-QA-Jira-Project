# 04. Test Cases

## Document Purpose

This document contains detailed test cases for manual testing of an existing e-commerce demo web application.

The test cases are based on:

- project overview;
- test strategy;
- functional checklist;
- common e-commerce user flows.

The goal is to verify critical user scenarios and prepare a base for Jira bug reporting.

---

## Test Case Status Legend

| Status              | Meaning                                      |
| ------------------- | -------------------------------------------- |
| Not Run             | Test case has not been executed yet          |
| Passed              | Actual result matches expected result        |
| Failed              | Actual result does not match expected result |
| Blocked             | Test case cannot be executed                 |
| Needs Clarification | Expected behavior requires clarification     |

---

## Test Environment

| Parameter   | Value                           |
| ----------- | ------------------------------- |
| Application | E-commerce demo web application |
| OS          | macOS                           |
| Browser     | Yandex Browser / Chrome         |
| Device      | Desktop / Laptop                |
| Test Type   | Manual functional testing       |
| Bug Tracker | Jira                            |
| Evidence    | Screenshots / videos            |

---

## TC-001: Open Home Page Successfully

| Field                | Value                       |
| -------------------- | --------------------------- |
| Test Case ID         | TC-001                      |
| Title                | Open home page successfully |
| Related Checklist ID | CHK-001, CHK-002, CHK-007   |
| Priority             | Critical                    |
| Type                 | Smoke / Functional          |
| Status               | Not Run                     |

### Preconditions

- Application URL is available.
- Browser is opened.

### Steps

1. Open the e-commerce demo application URL.
2. Wait until the page is fully loaded.
3. Check that the main page content is visible.
4. Check that header and navigation elements are displayed.
5. Open browser DevTools Console.
6. Check if critical console errors are present.

### Expected Result

- Home page opens successfully.
- Main navigation is visible.
- Main content is displayed.
- No critical layout issue is visible.
- No critical console errors appear during page load.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if the test fails.

---

## TC-002: Search Product by Valid Keyword

| Field                | Value                           |
| -------------------- | ------------------------------- |
| Test Case ID         | TC-002                          |
| Title                | Search product by valid keyword |
| Related Checklist ID | CHK-017, CHK-022, CHK-023       |
| Priority             | High                            |
| Type                 | Functional                      |
| Status               | Not Run                         |

### Preconditions

- Home page is opened.
- Search field is available.

### Test Data

| Field          | Value  |
| -------------- | ------ |
| Search Keyword | iphone |

### Steps

1. Click the search input field.
2. Enter valid product keyword: `iphone`.
3. Submit search.
4. Review search results.
5. Open one product from search results.

### Expected Result

- Search results page is opened.
- Search results are relevant to the entered keyword.
- Product name, price and image are visible if available.
- User can open product details page from search results.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if search results are incorrect or product cannot be opened.

---

## TC-003: Search Product by Non-Existing Keyword

| Field                | Value                                  |
| -------------------- | -------------------------------------- |
| Test Case ID         | TC-003                                 |
| Title                | Search product by non-existing keyword |
| Related Checklist ID | CHK-021                                |
| Priority             | Medium                                 |
| Type                 | Negative                               |
| Status               | Not Run                                |

### Preconditions

- Home page is opened.
- Search field is available.

### Test Data

| Field          | Value                |
| -------------- | -------------------- |
| Search Keyword | qwertytestproduct999 |

### Steps

1. Click the search input field.
2. Enter non-existing product keyword: `qwertytestproduct999`.
3. Submit search.
4. Review search results page.

### Expected Result

- Search results page is opened.
- System shows clear message that no products were found.
- Page does not break.
- No irrelevant products are displayed as exact results.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if behavior is incorrect.

---

## TC-004: Open Product Details Page

| Field                | Value                                       |
| -------------------- | ------------------------------------------- |
| Test Case ID         | TC-004                                      |
| Title                | Open product details page                   |
| Related Checklist ID | CHK-024, CHK-025, CHK-026, CHK-027, CHK-030 |
| Priority             | High                                        |
| Type                 | Functional / UI                             |
| Status               | Not Run                                     |

### Preconditions

- Product catalog or search results page is opened.
- At least one product is visible.

### Steps

1. Open product catalog or search results.
2. Click on a product card.
3. Wait until product details page is loaded.
4. Check product name.
5. Check product price.
6. Check product image.
7. Check Add to Cart button.

### Expected Result

- Product details page opens successfully.
- Product name is visible.
- Product price is visible.
- Product image is visible if available.
- Add to Cart button is visible and accessible.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if product page is broken or critical elements are missing.

---

## TC-005: Add Product to Cart from Product Details Page

| Field                | Value                                         |
| -------------------- | --------------------------------------------- |
| Test Case ID         | TC-005                                        |
| Title                | Add product to cart from product details page |
| Related Checklist ID | CHK-030, CHK-031, CHK-032, CHK-034            |
| Priority             | Critical                                      |
| Type                 | Functional                                    |
| Status               | Not Run                                       |

### Preconditions

- Product details page is opened.
- Product is available.
- Add to Cart button is visible.

### Steps

1. Open product details page.
2. Click Add to Cart button.
3. Check confirmation message if available.
4. Open cart page.
5. Verify that added product is displayed in cart.

### Expected Result

- Product is added to cart.
- User receives confirmation if confirmation behavior exists.
- Cart contains the added product.
- Product name and price in cart match product details page.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if product is not added to cart or cart data is incorrect.

---

## TC-006: Update Product Quantity in Cart

| Field                | Value                           |
| -------------------- | ------------------------------- |
| Test Case ID         | TC-006                          |
| Title                | Update product quantity in cart |
| Related Checklist ID | CHK-037, CHK-038, CHK-040       |
| Priority             | Critical                        |
| Type                 | Functional                      |
| Status               | Not Run                         |

### Preconditions

- Cart contains at least one product.
- Cart page is opened.

### Test Data

| Field        | Value |
| ------------ | ----- |
| New Quantity | 2     |

### Steps

1. Open cart page.
2. Find product quantity field.
3. Change product quantity to `2`.
4. Apply/update cart.
5. Check product subtotal.
6. Check cart total.

### Expected Result

- Product quantity is updated.
- Product subtotal is recalculated correctly.
- Cart total is recalculated correctly.
- No duplicate or unexpected cart item is created.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if quantity or total is calculated incorrectly.

---

## TC-007: Enter Invalid Product Quantity in Cart

| Field                | Value                                  |
| -------------------- | -------------------------------------- |
| Test Case ID         | TC-007                                 |
| Title                | Enter invalid product quantity in cart |
| Related Checklist ID | CHK-043, CHK-044, CHK-045              |
| Priority             | High                                   |
| Type                 | Negative / Validation                  |
| Status               | Not Run                                |

### Preconditions

- Cart contains at least one product.
- Cart page is opened.
- Quantity field is editable.

### Test Data

| Input Type        | Value  |
| ----------------- | ------ |
| Negative quantity | -1     |
| Zero quantity     | 0      |
| Text value        | abc    |
| Very large number | 999999 |

### Steps

1. Open cart page.
2. Enter invalid quantity value into quantity field.
3. Apply/update cart.
4. Observe system behavior.
5. Repeat steps for each invalid value.

### Expected Result

- System does not accept invalid quantity values.
- User sees clear validation message.
- Cart total is not calculated using invalid values.
- Application does not crash or show technical error.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if invalid quantity is accepted or cart behaves incorrectly.

---

## TC-008: Remove Product from Cart

| Field                | Value                    |
| -------------------- | ------------------------ |
| Test Case ID         | TC-008                   |
| Title                | Remove product from cart |
| Related Checklist ID | CHK-041, CHK-042         |
| Priority             | High                     |
| Type                 | Functional               |
| Status               | Not Run                  |

### Preconditions

- Cart contains at least one product.
- Cart page is opened.

### Steps

1. Open cart page.
2. Click remove/delete button for product.
3. Confirm removal if confirmation is shown.
4. Check cart content.

### Expected Result

- Product is removed from cart.
- Cart is updated correctly.
- If cart becomes empty, empty cart state is displayed.
- Cart total is updated correctly.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if product is not removed or cart state is incorrect.

---

## TC-009: Proceed from Cart to Checkout

| Field                | Value                         |
| -------------------- | ----------------------------- |
| Test Case ID         | TC-009                        |
| Title                | Proceed from cart to checkout |
| Related Checklist ID | CHK-046, CHK-047, CHK-048     |
| Priority             | Critical                      |
| Type                 | Functional                    |
| Status               | Not Run                       |

### Preconditions

- Cart contains at least one product.
- Cart page is opened.

### Steps

1. Open cart page.
2. Click Checkout or Proceed to Checkout button.
3. Wait until checkout page is opened.
4. Check that checkout form or checkout steps are displayed.
5. Check required fields.

### Expected Result

- User can proceed from cart to checkout.
- Checkout page opens successfully.
- Required checkout fields are visible.
- Order summary is displayed if available.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if checkout page is not accessible or required elements are missing.

---

## TC-010: Checkout with Empty Required Fields

| Field                | Value                               |
| -------------------- | ----------------------------------- |
| Test Case ID         | TC-010                              |
| Title                | Checkout with empty required fields |
| Related Checklist ID | CHK-049, CHK-055, CHK-065           |
| Priority             | Critical                            |
| Type                 | Negative / Validation               |
| Status               | Not Run                             |

### Preconditions

- Cart contains at least one product.
- Checkout page is opened.
- Required fields are available.

### Steps

1. Open checkout page.
2. Leave required fields empty.
3. Try to continue or submit checkout form.
4. Observe validation behavior.

### Expected Result

- Checkout cannot be completed with empty required fields.
- Validation messages are displayed for required fields.
- User understands what must be filled.
- No order is created with incomplete data.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if checkout allows empty required fields or validation is unclear.

---

## TC-011: Checkout with Invalid Email Format

| Field                | Value                              |
| -------------------- | ---------------------------------- |
| Test Case ID         | TC-011                             |
| Title                | Checkout with invalid email format |
| Related Checklist ID | CHK-050, CHK-067                   |
| Priority             | High                               |
| Type                 | Negative / Validation              |
| Status               | Not Run                            |

### Preconditions

- Checkout page is opened.
- Email field is available.

### Test Data

| Field | Value        |
| ----- | ------------ |
| Email | testuser     |
| Email | testuser@    |
| Email | testuser.com |

### Steps

1. Open checkout page.
2. Fill required fields with valid data except email.
3. Enter invalid email format.
4. Try to continue or submit checkout form.
5. Repeat for each invalid email value.

### Expected Result

- Invalid email format is rejected.
- Clear validation message is displayed.
- User cannot complete checkout with invalid email.
- No order is created with invalid email.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if invalid email is accepted.

---

## TC-012: Registration with Empty Required Fields

| Field                | Value                                   |
| -------------------- | --------------------------------------- |
| Test Case ID         | TC-012                                  |
| Title                | Registration with empty required fields |
| Related Checklist ID | CHK-057, CHK-058, CHK-059               |
| Priority             | High                                    |
| Type                 | Negative / Validation                   |
| Status               | Not Run                                 |

### Preconditions

- Registration page is available.

### Steps

1. Open registration page.
2. Leave required fields empty.
3. Try to submit registration form.
4. Observe validation messages.

### Expected Result

- Registration is not completed.
- Required fields are validated.
- Clear validation messages are displayed.
- User account is not created with incomplete data.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if registration allows missing required data or messages are unclear.

---

## TC-013: Login with Invalid Credentials

| Field                | Value                          |
| -------------------- | ------------------------------ |
| Test Case ID         | TC-013                         |
| Title                | Login with invalid credentials |
| Related Checklist ID | CHK-063                        |
| Priority             | High                           |
| Type                 | Negative / Functional          |
| Status               | Not Run                        |

### Preconditions

- Login page is available.

### Test Data

| Field    | Value                    |
| -------- | ------------------------ |
| Email    | invalid.user@example.com |
| Password | WrongPassword123         |

### Steps

1. Open login page.
2. Enter invalid email and password.
3. Submit login form.
4. Observe system response.

### Expected Result

- Login is rejected.
- User remains unauthenticated.
- Clear error message is displayed.
- No unexpected technical error appears.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if login behavior is incorrect.

---

## TC-014: Basic Mobile Viewport Check for Product and Cart Flow

| Field                | Value                                                 |
| -------------------- | ----------------------------------------------------- |
| Test Case ID         | TC-014                                                |
| Title                | Basic mobile viewport check for product and cart flow |
| Related Checklist ID | CHK-072, CHK-075, CHK-076, CHK-077, CHK-079, CHK-080  |
| Priority             | High                                                  |
| Type                 | Responsive Web Testing                                |
| Status               | Not Run                                               |

### Preconditions

- Browser DevTools is available.
- Mobile viewport mode is enabled.

### Test Data

| Parameter | Value                                |
| --------- | ------------------------------------ |
| Viewport  | Mobile viewport, for example 390x844 |
| Flow      | Product details → Add to Cart → Cart |

### Steps

1. Open application in browser.
2. Enable mobile viewport in DevTools.
3. Open product details page.
4. Check that product information is readable.
5. Check that Add to Cart button is visible and accessible.
6. Add product to cart.
7. Open cart page.
8. Check that cart page is usable.
9. Check that no unexpected horizontal scrolling or overlapping elements appear.

### Expected Result

- Product page is usable on mobile viewport.
- Add to Cart button is accessible.
- Cart page is usable.
- No critical overlapping elements appear.
- No unexpected horizontal scrolling appears.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if mobile layout is broken.

---

## TC-015: Browser Console Check During Critical Cart Flow

| Field                | Value                                           |
| -------------------- | ----------------------------------------------- |
| Test Case ID         | TC-015                                          |
| Title                | Browser console check during critical cart flow |
| Related Checklist ID | CHK-082, CHK-084, CHK-085, CHK-087              |
| Priority             | Medium                                          |
| Type                 | DevTools / Investigation                        |
| Status               | Not Run                                         |

### Preconditions

- Browser DevTools is available.
- Application is opened.

### Steps

1. Open browser DevTools.
2. Open Console tab.
3. Open product details page.
4. Add product to cart.
5. Open cart page.
6. Proceed to checkout if available.
7. Check Console tab for critical errors.
8. Open Network tab and check if critical requests fail.

### Expected Result

- No critical console errors appear during product/cart/checkout flow.
- No critical failed network requests break the user flow.
- Product/cart/checkout flow remains usable.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if critical console or network errors are found.

---

## TC-016: Refresh Cart Page After Adding Product

| Field                | Value                                  |
| -------------------- | -------------------------------------- |
| Test Case ID         | TC-016                                 |
| Title                | Refresh cart page after adding product |
| Related Checklist ID | CHK-034, CHK-094                       |
| Priority             | Medium                                 |
| Type                 | Exploratory / Functional               |
| Status               | Not Run                                |

### Preconditions

- Product was added to cart.
- Cart page is opened.

### Steps

1. Open cart page with added product.
2. Refresh the page.
3. Check cart content after refresh.
4. Check product quantity and total.

### Expected Result

- Cart state is preserved after page refresh.
- Added product remains in cart.
- Product quantity remains correct.
- Cart total remains correct.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if cart state is lost or recalculated incorrectly.

---

## TC-017: Use Browser Back Button During Checkout Flow

| Field                | Value                                        |
| -------------------- | -------------------------------------------- |
| Test Case ID         | TC-017                                       |
| Title                | Use browser Back button during checkout flow |
| Related Checklist ID | CHK-090                                      |
| Priority             | Medium                                       |
| Type                 | Exploratory / Functional                     |
| Status               | Not Run                                      |

### Preconditions

- Cart contains at least one product.
- Checkout page is opened.

### Steps

1. Open checkout page.
2. Fill several checkout fields.
3. Click browser Back button.
4. Return to checkout page.
5. Check whether entered data and cart state are handled correctly.

### Expected Result

- Application does not crash.
- Cart state remains correct.
- User can continue checkout or clearly understands that data was reset.
- No technical error page appears.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if checkout state is broken.

---

## TC-018: Repeated Clicks on Add to Cart Button

| Field                | Value                                 |
| -------------------- | ------------------------------------- |
| Test Case ID         | TC-018                                |
| Title                | Repeated clicks on Add to Cart button |
| Related Checklist ID | CHK-088                               |
| Priority             | Medium                                |
| Type                 | Exploratory / Negative                |
| Status               | Not Run                               |

### Preconditions

- Product details page is opened.
- Add to Cart button is visible.

### Steps

1. Click Add to Cart button several times quickly.
2. Open cart page.
3. Check product quantity.
4. Check cart total.
5. Check whether duplicate unexpected items are created.

### Expected Result

- System handles repeated clicks correctly.
- Cart quantity and total are predictable.
- No unexpected duplicates are created.
- No technical error appears.

### Actual Result

To be filled during test execution.

### Evidence

To be attached if repeated clicks cause incorrect cart behavior.

---

## Test Execution Notes

- Test cases with `Critical` priority should be executed first.
- Failed test cases should be reported in Jira.
- Screenshots or video evidence should be attached to each confirmed bug.
- DevTools Console and Network information should be added when relevant.
- If expected behavior is unclear, the case should be marked as `Needs Clarification`.

---

## Coverage Summary

| Area             | Covered By                     |
| ---------------- | ------------------------------ |
| Home page        | TC-001                         |
| Search           | TC-002, TC-003                 |
| Product details  | TC-004                         |
| Add to cart      | TC-005, TC-018                 |
| Cart quantity    | TC-006, TC-007                 |
| Remove from cart | TC-008                         |
| Checkout         | TC-009, TC-010, TC-011, TC-017 |
| Registration     | TC-012                         |
| Login            | TC-013                         |
| Mobile viewport  | TC-014                         |
| DevTools checks  | TC-015                         |
| Cart persistence | TC-016                         |
