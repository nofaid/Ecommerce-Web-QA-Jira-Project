# 01. Project Overview

## Project Name

E-commerce Web QA Jira Project

## Application Under Test

Application: nopCommerce Demo Store  
URL: https://demo.nopcommerce.com/  
Application type: Existing e-commerce demo web application

## Business Context

An e-commerce application allows users to browse products, search for items, view product details, add products to cart and complete checkout.

For this type of system, quality is important because defects may affect:

- product discovery;
- cart behavior;
- checkout completion;
- user registration;
- customer trust;
- order conversion;
- business revenue.

Even small issues in cart, checkout or validation logic may cause users to abandon the purchase flow.

## QA Context

The QA engineer verifies that the main user flows work correctly and that defects are reported clearly with evidence.

The focus of this project is not only to find bugs, but also to demonstrate a realistic QA process:

- define test scope;
- prepare checklist;
- design test cases;
- execute manual checks;
- create Jira bug reports;
- attach evidence;
- summarize test results.

## Application Areas

| Area                 | Description                                                     |
| -------------------- | --------------------------------------------------------------- |
| Home Page            | Main entry point of the e-commerce application                  |
| Catalog              | Product listing and category navigation                         |
| Product Details      | Product information, price, availability and add-to-cart action |
| Search               | Product search by keyword                                       |
| Cart                 | Added products, quantity update, removal and total calculation  |
| Checkout             | Customer data, delivery/payment steps and order confirmation    |
| Registration / Login | User account creation and authentication                        |
| Forms                | Required fields, validation and error messages                  |
| Mobile Layout        | Basic responsiveness on smaller screen sizes                    |
| Browser DevTools     | Console errors and failed network requests                      |

## QA Scope

Testing scope includes:

- manual functional testing;
- UI validation;
- form validation;
- positive scenarios;
- negative scenarios;
- cart and checkout checks;
- exploratory testing;
- basic mobile viewport testing;
- browser console checks;
- Jira bug reporting;
- evidence collection;
- test summary preparation.

## Out of Scope

The following areas are not covered:

- real payment processing;
- load testing;
- performance testing;
- security testing;
- automated testing;
- backend database testing;
- direct API testing;
- production environment testing.

## Test Approach

The testing approach includes:

1. Review main e-commerce flows.
2. Create checklist based on user scenarios.
3. Prepare test cases for critical flows.
4. Execute manual tests.
5. Investigate unexpected behavior.
6. Create Jira bug reports.
7. Attach screenshots or video evidence.
8. Summarize results in test summary.

## Jira Usage

Jira is used to simulate a real bug tracking workflow.

Bug reports include:

- summary;
- description;
- steps to reproduce;
- expected result;
- actual result;
- severity;
- priority;
- environment;
- attachments;
- status.

Basic workflow:

    To Do → In Progress → Ready for Retest → Done

If the Jira project does not support custom statuses, the simplified workflow can be used:

    To Do → In Progress → Done

## Main User Flows

| Flow ID  | User Flow                                      | Priority |
| -------- | ---------------------------------------------- | -------- |
| FLOW-001 | Open home page and navigate to product catalog | High     |
| FLOW-002 | Search for product by keyword                  | High     |
| FLOW-003 | Open product details page                      | High     |
| FLOW-004 | Add product to cart                            | Critical |
| FLOW-005 | Update product quantity in cart                | Critical |
| FLOW-006 | Remove product from cart                       | High     |
| FLOW-007 | Complete checkout flow                         | Critical |
| FLOW-008 | Register new user account                      | High     |
| FLOW-009 | Login with existing account                    | High     |
| FLOW-010 | Check form validation for invalid data         | High     |
| FLOW-011 | Check mobile viewport layout                   | Medium   |
| FLOW-012 | Check browser console for visible errors       | Medium   |

## Key Quality Risks

| Risk                                       | Possible Impact                           |
| ------------------------------------------ | ----------------------------------------- |
| Product cannot be added to cart            | User cannot start purchase flow           |
| Cart quantity is calculated incorrectly    | User may see wrong order total            |
| Checkout validation is weak                | Incorrect customer data may be accepted   |
| Required fields are not validated          | Order may be created with incomplete data |
| Search does not return relevant products   | User may not find needed item             |
| Mobile layout is broken                    | Mobile users may abandon the site         |
| Console errors appear during critical flow | Hidden frontend issues may exist          |
| Bug report lacks evidence                  | Developer may not reproduce the issue     |

## Expected Project Result

At the end of the project, the repository should contain:

- project overview;
- test strategy;
- checklist;
- test cases;
- Jira bug report examples;
- evidence folder;
- test summary;
- retrospective.

The Jira project should contain created bug reports with clear reproduction steps and attached evidence.
