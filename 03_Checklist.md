# 03. Checklist

## Document Purpose

This checklist is used for manual testing of an existing e-commerce demo web application.

The checklist covers:

- home page;
- product catalog;
- search;
- product details page;
- cart;
- checkout;
- registration and login;
- form validation;
- mobile viewport;
- browser DevTools checks.

The goal is to verify main user flows and identify functional, UI and validation issues.

---

## Checklist Status Legend

| Status              | Meaning                                      |
| ------------------- | -------------------------------------------- |
| Not Run             | Check has not been executed yet              |
| Passed              | Actual result matches expected result        |
| Failed              | Actual result does not match expected result |
| Blocked             | Check cannot be executed                     |
| Needs Clarification | Expected behavior is unclear                 |

---

## Priority Legend

| Priority | Meaning                                    |
| -------- | ------------------------------------------ |
| Critical | Critical purchase/user flow may be blocked |
| High     | Important functionality or user flow       |
| Medium   | Useful but not critical functionality      |
| Low      | Low-risk or cosmetic area                  |

---

## Home Page

| ID      | Check                                                         | Priority | Status  | Notes |
| ------- | ------------------------------------------------------------- | -------- | ------- | ----- |
| CHK-001 | Verify that home page opens successfully                      | Critical | Not Run |       |
| CHK-002 | Verify that main navigation menu is visible                   | High     | Not Run |       |
| CHK-003 | Verify that product categories are visible or accessible      | High     | Not Run |       |
| CHK-004 | Verify that featured products or product blocks are displayed | Medium   | Not Run |       |
| CHK-005 | Verify that header elements are displayed correctly           | Medium   | Not Run |       |
| CHK-006 | Verify that footer elements are displayed correctly           | Low      | Not Run |       |
| CHK-007 | Verify that main page does not show obvious layout issues     | High     | Not Run |       |

---

## Product Catalog

| ID      | Check                                               | Priority | Status  | Notes |
| ------- | --------------------------------------------------- | -------- | ------- | ----- |
| CHK-008 | Verify that product catalog page opens successfully | High     | Not Run |       |
| CHK-009 | Verify that product list is displayed               | High     | Not Run |       |
| CHK-010 | Verify that product cards contain product name      | High     | Not Run |       |
| CHK-011 | Verify that product cards contain product price     | High     | Not Run |       |
| CHK-012 | Verify that product image is displayed              | Medium   | Not Run |       |
| CHK-013 | Verify that product card can be opened              | High     | Not Run |       |
| CHK-014 | Verify that category navigation works correctly     | Medium   | Not Run |       |
| CHK-015 | Verify that sorting works if available              | Medium   | Not Run |       |
| CHK-016 | Verify that pagination works if available           | Medium   | Not Run |       |

---

## Search

| ID      | Check                                                 | Priority | Status  | Notes |
| ------- | ----------------------------------------------------- | -------- | ------- | ----- |
| CHK-017 | Verify search with valid product keyword              | High     | Not Run |       |
| CHK-018 | Verify search with partial product keyword            | Medium   | Not Run |       |
| CHK-019 | Verify search with uppercase/lowercase input          | Medium   | Not Run |       |
| CHK-020 | Verify search with empty input                        | Medium   | Not Run |       |
| CHK-021 | Verify search with non-existing product keyword       | Medium   | Not Run |       |
| CHK-022 | Verify that search results contain relevant products  | High     | Not Run |       |
| CHK-023 | Verify that user can open product from search results | High     | Not Run |       |

---

## Product Details Page

| ID      | Check                                                               | Priority | Status  | Notes |
| ------- | ------------------------------------------------------------------- | -------- | ------- | ----- |
| CHK-024 | Verify that product details page opens successfully                 | High     | Not Run |       |
| CHK-025 | Verify that product name is displayed                               | High     | Not Run |       |
| CHK-026 | Verify that product price is displayed                              | High     | Not Run |       |
| CHK-027 | Verify that product image is displayed                              | Medium   | Not Run |       |
| CHK-028 | Verify that product description is displayed                        | Medium   | Not Run |       |
| CHK-029 | Verify that product availability is displayed if available          | Medium   | Not Run |       |
| CHK-030 | Verify that Add to Cart button is visible                           | Critical | Not Run |       |
| CHK-031 | Verify that product can be added to cart                            | Critical | Not Run |       |
| CHK-032 | Verify that user receives confirmation after adding product to cart | High     | Not Run |       |

---

## Cart

| ID      | Check                                                         | Priority | Status  | Notes |
| ------- | ------------------------------------------------------------- | -------- | ------- | ----- |
| CHK-033 | Verify that cart page opens successfully                      | Critical | Not Run |       |
| CHK-034 | Verify that added product is displayed in cart                | Critical | Not Run |       |
| CHK-035 | Verify that product name is correct in cart                   | High     | Not Run |       |
| CHK-036 | Verify that product price is correct in cart                  | High     | Not Run |       |
| CHK-037 | Verify that product quantity is displayed                     | High     | Not Run |       |
| CHK-038 | Verify that product quantity can be increased                 | High     | Not Run |       |
| CHK-039 | Verify that product quantity can be decreased                 | High     | Not Run |       |
| CHK-040 | Verify that cart total is recalculated after quantity change  | Critical | Not Run |       |
| CHK-041 | Verify that product can be removed from cart                  | High     | Not Run |       |
| CHK-042 | Verify that empty cart state is displayed correctly           | Medium   | Not Run |       |
| CHK-043 | Verify that cart does not accept invalid quantity value       | High     | Not Run |       |
| CHK-044 | Verify that cart does not accept negative quantity value      | High     | Not Run |       |
| CHK-045 | Verify that cart does not accept zero quantity if not allowed | Medium   | Not Run |       |

---

## Checkout

| ID      | Check                                                                              | Priority | Status  | Notes |
| ------- | ---------------------------------------------------------------------------------- | -------- | ------- | ----- |
| CHK-046 | Verify that user can proceed from cart to checkout                                 | Critical | Not Run |       |
| CHK-047 | Verify that checkout page opens successfully                                       | Critical | Not Run |       |
| CHK-048 | Verify that required checkout fields are displayed                                 | High     | Not Run |       |
| CHK-049 | Verify that required checkout fields cannot be empty                               | Critical | Not Run |       |
| CHK-050 | Verify that invalid email format is rejected                                       | High     | Not Run |       |
| CHK-051 | Verify that invalid phone number is rejected if phone validation exists            | High     | Not Run |       |
| CHK-052 | Verify that address field is required                                              | High     | Not Run |       |
| CHK-053 | Verify that delivery/payment options are displayed if available                    | High     | Not Run |       |
| CHK-054 | Verify that order total is displayed correctly at checkout                         | Critical | Not Run |       |
| CHK-055 | Verify that user cannot complete checkout with missing required data               | Critical | Not Run |       |
| CHK-056 | Verify that order confirmation is displayed after successful checkout if available | Critical | Not Run |       |

---

## Registration and Login

| ID      | Check                                                                | Priority | Status  | Notes |
| ------- | -------------------------------------------------------------------- | -------- | ------- | ----- |
| CHK-057 | Verify that registration page opens successfully                     | High     | Not Run |       |
| CHK-058 | Verify that required registration fields are displayed               | High     | Not Run |       |
| CHK-059 | Verify that registration form validates empty required fields        | High     | Not Run |       |
| CHK-060 | Verify that invalid email format is rejected during registration     | High     | Not Run |       |
| CHK-061 | Verify that password confirmation is validated if available          | High     | Not Run |       |
| CHK-062 | Verify that user can log in with valid credentials if account exists | High     | Not Run |       |
| CHK-063 | Verify that login with invalid credentials is rejected               | High     | Not Run |       |
| CHK-064 | Verify that logout works correctly if available                      | Medium   | Not Run |       |

---

## Form Validation

| ID      | Check                                                                                   | Priority | Status  | Notes |
| ------- | --------------------------------------------------------------------------------------- | -------- | ------- | ----- |
| CHK-065 | Verify that required fields show validation messages                                    | High     | Not Run |       |
| CHK-066 | Verify that validation messages are clear and readable                                  | Medium   | Not Run |       |
| CHK-067 | Verify that email fields reject invalid format                                          | High     | Not Run |       |
| CHK-068 | Verify that phone fields reject invalid characters if validation exists                 | Medium   | Not Run |       |
| CHK-069 | Verify that name fields handle numbers and special characters according to requirements | Medium   | Not Run |       |
| CHK-070 | Verify that long input values do not break layout                                       | Medium   | Not Run |       |
| CHK-071 | Verify that leading/trailing spaces are handled correctly                               | Low      | Not Run |       |

---

## Mobile Viewport

| ID      | Check                                                           | Priority | Status  | Notes |
| ------- | --------------------------------------------------------------- | -------- | ------- | ----- |
| CHK-072 | Verify that home page is usable on mobile viewport              | High     | Not Run |       |
| CHK-073 | Verify that navigation menu works on mobile viewport            | High     | Not Run |       |
| CHK-074 | Verify that product cards are readable on mobile viewport       | Medium   | Not Run |       |
| CHK-075 | Verify that product details page is usable on mobile viewport   | High     | Not Run |       |
| CHK-076 | Verify that Add to Cart button is accessible on mobile viewport | Critical | Not Run |       |
| CHK-077 | Verify that cart page is usable on mobile viewport              | Critical | Not Run |       |
| CHK-078 | Verify that checkout form is usable on mobile viewport          | Critical | Not Run |       |
| CHK-079 | Verify that no horizontal scrolling appears unexpectedly        | Medium   | Not Run |       |
| CHK-080 | Verify that buttons are not overlapped on mobile viewport       | High     | Not Run |       |
| CHK-081 | Verify that validation messages are visible on mobile viewport  | High     | Not Run |       |

---

## Browser DevTools Checks

| ID      | Check                                                                     | Priority | Status  | Notes |
| ------- | ------------------------------------------------------------------------- | -------- | ------- | ----- |
| CHK-082 | Verify that no critical console errors appear on home page                | Medium   | Not Run |       |
| CHK-083 | Verify that no critical console errors appear during product search       | Medium   | Not Run |       |
| CHK-084 | Verify that no critical console errors appear when adding product to cart | High     | Not Run |       |
| CHK-085 | Verify that no critical console errors appear during checkout flow        | High     | Not Run |       |
| CHK-086 | Verify that product images are not broken                                 | Medium   | Not Run |       |
| CHK-087 | Verify that no obvious failed network requests affect critical flows      | Medium   | Not Run |       |

---

## Exploratory Testing Ideas

| ID      | Check                                                   | Priority | Status  | Notes |
| ------- | ------------------------------------------------------- | -------- | ------- | ----- |
| CHK-088 | Try repeated clicks on Add to Cart button               | Medium   | Not Run |       |
| CHK-089 | Change cart quantity several times quickly              | Medium   | Not Run |       |
| CHK-090 | Use browser Back button during checkout flow            | Medium   | Not Run |       |
| CHK-091 | Remove product from cart and return to product page     | Medium   | Not Run |       |
| CHK-092 | Search for product and then add it to cart from results | High     | Not Run |       |
| CHK-093 | Open cart in another tab if possible                    | Low      | Not Run |       |
| CHK-094 | Refresh cart page after quantity update                 | Medium   | Not Run |       |
| CHK-095 | Refresh checkout page after entering partial data       | Medium   | Not Run |       |

---

## Critical Smoke Checklist

This short checklist can be used for quick smoke testing.

| ID      | Check                                   | Priority | Status  |
| ------- | --------------------------------------- | -------- | ------- |
| SMK-001 | Home page opens successfully            | Critical | Not Run |
| SMK-002 | Product catalog is accessible           | Critical | Not Run |
| SMK-003 | Product details page opens successfully | Critical | Not Run |
| SMK-004 | Product can be added to cart            | Critical | Not Run |
| SMK-005 | Cart page displays added product        | Critical | Not Run |
| SMK-006 | Cart total is displayed                 | Critical | Not Run |
| SMK-007 | Checkout page is accessible             | Critical | Not Run |
| SMK-008 | Required checkout fields are validated  | Critical | Not Run |

---

## Notes

- Failed checks should be reported in Jira as bugs.
- Checks with unclear expected behavior should be documented in test notes.
- Evidence should be attached for every confirmed bug.
- Mobile viewport checks are basic responsive web checks, not full native mobile testing.
- DevTools checks are used only for visible errors and investigation.
