# 02. Test Strategy

## Application Under Test

Application: nopCommerce Demo Store  
URL: https://demo.nopcommerce.com/  
Application type: Existing e-commerce demo web application.

The application allows users to:

- browse products;
- search for products;
- open product details;
- add products to cart;
- update cart quantity;
- remove products from cart;
- proceed to checkout;
- register or log in;
- fill customer/order forms.

## Testing Goal

The main goal of testing is to verify that critical e-commerce user flows work correctly and that any found defects are documented in Jira with clear evidence.

Special attention is paid to:

- product search;
- product details page;
- cart behavior;
- checkout flow;
- form validation;
- mobile layout;
- visible UI issues;
- browser console errors;
- user flow interruptions.

---

## Testing Scope

The testing scope includes:

| Area                 | Included                           |
| -------------------- | ---------------------------------- |
| Home page            | Yes                                |
| Product catalog      | Yes                                |
| Product search       | Yes                                |
| Product details page | Yes                                |
| Cart                 | Yes                                |
| Checkout flow        | Yes                                |
| Registration / Login | Yes, if available                  |
| Form validation      | Yes                                |
| Mobile viewport      | Basic checks                       |
| Browser console      | Basic checks                       |
| Network tab          | Basic visible failed requests only |

---

## Out of Scope

The following areas are not covered:

| Area                     | Reason                                                   |
| ------------------------ | -------------------------------------------------------- |
| Load testing             | Not safe for public/demo systems                         |
| Performance testing      | Not part of current manual QA scope                      |
| Security testing         | Not allowed without permission                           |
| Penetration testing      | Not allowed without permission                           |
| Real payment testing     | No real payment operations should be performed           |
| Backend database testing | No database access                                       |
| API testing              | Not part of this project                                 |
| Automation testing       | This project focuses on manual QA and Jira bug reporting |

---

## Testing Types

## Functional Testing

Functional testing is used to verify that main e-commerce features work according to expected user behavior.

Examples:

- user can search for a product;
- user can open product details;
- user can add product to cart;
- cart total is updated correctly;
- user can proceed to checkout.

---

## UI Testing

UI testing is used to verify that important interface elements are visible, readable and usable.

Examples:

- buttons are visible;
- product price is displayed;
- form fields are readable;
- error messages are understandable;
- layout is not broken.

---

## Validation Testing

Validation testing is used to verify that forms correctly handle valid and invalid input.

Examples:

- required fields cannot be empty;
- email field validates email format;
- phone field does not accept invalid characters;
- quantity field does not accept invalid values.

---

## Negative Testing

Negative testing is used to verify that the system handles invalid actions correctly.

Examples:

- checkout with empty required fields;
- invalid email during registration;
- invalid product quantity;
- removing all items from cart;
- trying to proceed without required data.

---

## Exploratory Testing

Exploratory testing is used to find unexpected issues that may not be covered by predefined test cases.

Examples:

- unusual navigation paths;
- repeated clicks;
- browser back/forward behavior;
- changing cart quantity several times;
- switching between product pages and cart.

---

## Basic Regression Testing

Basic regression testing is used after a bug is fixed or after changes in critical areas.

Regression focus areas:

- search;
- product page;
- cart;
- checkout;
- validation;
- previously reported bugs.

---

## Mobile Viewport Testing

Basic mobile viewport testing is used to verify that the application remains usable on smaller screen sizes.

Checked areas:

- header;
- menu;
- product cards;
- cart;
- checkout forms;
- buttons;
- error messages.

This is not full mobile application testing. It is responsive web testing.

---

## Browser DevTools Checks

Browser DevTools are used for basic investigation.

Checked areas:

- Console errors;
- failed Network requests;
- broken images;
- unexpected frontend errors during critical flows.

DevTools checks are used only for observation and evidence collection.

---

## Test Environment

| Parameter   | Value                         |
| ----------- | ----------------------------- |
| OS          | macOS                         |
| Browser     | Yandex Browser / Chrome       |
| Device      | Desktop / Laptop              |
| Application | nopCommerce Demo Store        |
| URL         | https://demo.nopcommerce.com/ |
| Test Type   | Manual testing                |
| Bug Tracker | Jira                          |
| Evidence    | Screenshots / videos          |

---

## Test Data

Only safe test data should be used.

Examples:

| Field       | Test Data             |
| ----------- | --------------------- |
| First Name  | Test                  |
| Last Name   | User                  |
| Email       | test.user@example.com |
| Phone       | +77010000001          |
| Address     | Test Street 1         |
| City        | Almaty                |
| Postal Code | 050000                |

No real personal data should be used.

---

## Defect Reporting Approach

All confirmed defects should be created in Jira.

Each Jira bug should include:

- clear summary;
- affected area;
- environment;
- preconditions;
- steps to reproduce;
- expected result;
- actual result;
- severity;
- priority;
- attachments;
- related test case, if applicable.

---

## Jira Workflow

Preferred workflow:

    To Do → In Progress → Ready for Retest → Done

If custom statuses are not available, simplified workflow can be used:

    To Do → In Progress → Done

---

## Bug Severity

| Severity | Meaning                                                    |
| -------- | ---------------------------------------------------------- |
| Critical | Critical user flow is blocked or data/order flow is broken |
| Major    | Important functionality works incorrectly                  |
| Minor    | Non-critical functional or UI issue                        |
| Trivial  | Cosmetic issue with very low impact                        |

---

## Bug Priority

| Priority | Meaning                                                     |
| -------- | ----------------------------------------------------------- |
| High     | Should be fixed soon because it affects important user flow |
| Medium   | Should be fixed in planned scope                            |
| Low      | Can be fixed later                                          |

---

## Evidence Requirements

Good bug evidence should include at least one of the following:

- screenshot;
- video recording;
- browser console screenshot;
- network error screenshot;
- clear actual result description.

Evidence should be stored in:

- Jira attachment;
- GitHub `evidence` folder.

Recommended evidence naming:

    BUG-001_checkout_required_field_validation.png
    BUG-002_cart_quantity_update_error.mp4
    BUG-003_mobile_layout_broken.png

---

## Entry Criteria

Testing can start when:

- application is accessible;
- main user flows are identified;
- checklist is prepared;
- test environment is ready;
- Jira project is created;
- evidence folder is prepared.

---

## Exit Criteria

Testing can be considered complete when:

- checklist is executed;
- critical test cases are executed;
- found bugs are reported in Jira;
- evidence is attached;
- test summary is prepared;
- main risks are documented.

---

## Main Testing Risks

| Risk                                     | Impact                                       | Mitigation                                               |
| ---------------------------------------- | -------------------------------------------- | -------------------------------------------------------- |
| Demo application may change unexpectedly | Test results may become outdated             | Document test date and environment                       |
| Some flows may be unavailable            | Test coverage may be incomplete              | Mark checks as blocked or out of scope                   |
| No real backend/database access          | Data validation is limited                   | Focus on UI and user flow behavior                       |
| Jira project is self-managed             | It does not prove commercial Jira experience | Clearly state that Jira is used for portfolio simulation |
| No real bug fixes                        | Retest may be simulated                      | Document bug status and retest approach clearly          |

---

## QA Notes

- Testing should be ethical and safe.
- No load, security or destructive testing should be performed.
- Only demo/test data should be used.
- All bugs should be documented clearly and professionally.
- The goal is not to find as many bugs as possible, but to demonstrate a realistic QA process.
