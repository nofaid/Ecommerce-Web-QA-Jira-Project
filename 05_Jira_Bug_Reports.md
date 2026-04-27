# 05. Jira Bug Reports

## Document Purpose

This document contains a public summary of bugs reported in Jira during manual testing of an existing e-commerce demo web application.

The full bug reports are created in Jira.

This GitHub document is used to show:

- bug summary;
- affected area;
- severity and priority;
- steps to reproduce;
- expected result;
- actual result;
- evidence links;
- Jira workflow status.

---

## Important Note

Bugs in this document should be based only on real test execution results.

No fake bugs should be added.

Each bug should have:

- Jira issue;
- clear reproduction steps;
- actual result;
- expected result;
- evidence;
- environment information.

---

## Jira Project Information

| Field             | Value                           |
| ----------------- | ------------------------------- |
| Jira Project Name | E-commerce Web QA Testing       |
| Project Type      | Kanban                          |
| Issue Type        | Bug                             |
| Testing Type      | Manual Testing                  |
| Application Type  | E-commerce demo web application |
| Evidence          | Screenshots / Videos            |
| Public Summary    | GitHub repository               |

---

## Jira Bug Workflow

Preferred workflow:

    To Do → In Progress → Ready for Retest → Done

If custom statuses are not available, simplified workflow can be used:

    To Do → In Progress → Done

---

## Bug Report Fields

Each Jira bug should contain:

| Field              | Description                          |
| ------------------ | ------------------------------------ |
| Summary            | Short and clear bug title            |
| Description        | Brief explanation of the issue       |
| Steps to Reproduce | Step-by-step reproduction path       |
| Expected Result    | What should happen                   |
| Actual Result      | What actually happens                |
| Severity           | Business/technical impact            |
| Priority           | Fix urgency                          |
| Environment        | Browser, OS, application, device     |
| Attachments        | Screenshot or video evidence         |
| Labels             | Area and type of issue               |
| Related Test Case  | Test case ID from `04_Test_Cases.md` |

---

## Severity Levels

| Severity | Meaning                                                             |
| -------- | ------------------------------------------------------------------- |
| Critical | Critical user flow is blocked or order/cart/checkout flow is broken |
| Major    | Important functionality works incorrectly                           |
| Minor    | Non-critical issue with limited impact                              |
| Trivial  | Cosmetic issue with very low impact                                 |

---

## Priority Levels

| Priority | Meaning                                                      |
| -------- | ------------------------------------------------------------ |
| High     | Should be fixed soon because important user flow is affected |
| Medium   | Should be fixed in planned scope                             |
| Low      | Can be fixed later                                           |

---

## Bug Labels

Recommended Jira labels:

| Label          | Meaning                        |
| -------------- | ------------------------------ |
| ecommerce      | E-commerce application issue   |
| manual-testing | Found during manual testing    |
| web-testing    | Web application issue          |
| ui             | UI issue                       |
| validation     | Form or input validation issue |
| cart           | Cart-related issue             |
| checkout       | Checkout-related issue         |
| search         | Search-related issue           |
| mobile         | Mobile viewport issue          |
| devtools       | Console or Network issue       |
| regression     | Regression-related issue       |

---

## Bug Summary Table

| Bug ID  | Jira Key     | Summary                         | Area         | Severity     | Priority     | Status       | Evidence     |
| ------- | ------------ | ------------------------------- | ------------ | ------------ | ------------ | ------------ | ------------ |
| BUG-001 | To be filled | To be filled after real testing | To be filled | To be filled | To be filled | To be filled | To be filled |
| BUG-002 | To be filled | To be filled after real testing | To be filled | To be filled | To be filled | To be filled | To be filled |
| BUG-003 | To be filled | To be filled after real testing | To be filled | To be filled | To be filled | To be filled | To be filled |

---

# Bug Report Template

Use this template for each confirmed bug.

---

## BUG-XXX: Bug Title

| Field             | Value        |
| ----------------- | ------------ |
| Bug ID            | BUG-XXX      |
| Jira Key          | To be filled |
| Type              | Bug          |
| Status            | To Do        |
| Severity          | To be filled |
| Priority          | To be filled |
| Area              | To be filled |
| Related Test Case | To be filled |
| Environment       | To be filled |
| Evidence          | To be filled |

### Summary

Short description of the issue.

### Preconditions

- Preconditions should be listed here.
- Example: Product is added to cart.
- Example: Checkout page is opened.

### Steps to Reproduce

1. Step 1.
2. Step 2.
3. Step 3.
4. Step 4.

### Expected Result

Describe what should happen.

### Actual Result

Describe what actually happens.

### Evidence

Add links to evidence files:

- screenshot;
- video;
- console screenshot;
- network screenshot.

### Impact

Describe why this issue matters for the user or business.

### QA Comment

Add additional QA notes if needed.

---

# Example Bug Format

This example shows the expected format. It should be replaced with real bugs after test execution.

---

## BUG-EXAMPLE: Checkout Allows Submitting Form with Empty Required Field

| Field             | Value                          |
| ----------------- | ------------------------------ |
| Bug ID            | BUG-EXAMPLE                    |
| Jira Key          | Example only                   |
| Type              | Bug                            |
| Status            | To Do                          |
| Severity          | Major                          |
| Priority          | High                           |
| Area              | Checkout / Validation          |
| Related Test Case | TC-010                         |
| Environment       | macOS, Yandex Browser / Chrome |
| Evidence          | Example only                   |

### Summary

Checkout form allows the user to continue without filling a required field.

### Preconditions

- Product is added to cart.
- Checkout page is opened.

### Steps to Reproduce

1. Open cart page.
2. Proceed to checkout.
3. Leave required field empty.
4. Try to continue checkout.

### Expected Result

System should block checkout and show validation message for the required field.

### Actual Result

System allows the user to continue without required field validation.

### Evidence

Example only.

### Impact

User may create an order with incomplete customer or delivery data.

### QA Comment

This is an example format. Real bugs should be added only after actual test execution.

---

## Current Bug Execution Notes

| Item                          | Status        |
| ----------------------------- | ------------- |
| Jira project created          | To be updated |
| Checklist prepared            | Done          |
| Test cases prepared           | Done          |
| Manual test execution started | To be updated |
| First bug reported in Jira    | To be updated |
| Evidence attached             | To be updated |
| GitHub bug summary updated    | To be updated |

---

## QA Rules for This Project

- Do not add fake bugs.
- Do not report behavior as a bug if expected result is unclear.
- If expected behavior is unclear, document it as a question or note.
- Every confirmed bug should have evidence.
- Every bug should be reproducible.
- Every bug should have clear expected and actual result.
- Severity should describe impact.
- Priority should describe urgency.

## Bug Summary

During the first test execution session, no confirmed functional bugs were found.

| Session   | Area                        | Result                   |
| --------- | --------------------------- | ------------------------ |
| Session 1 | Smoke flow                  | Passed                   |
| Session 1 | Product search              | Passed                   |
| Session 1 | Product details             | Passed                   |
| Session 1 | Add to cart                 | Passed                   |
| Session 1 | Cart quantity validation    | Passed                   |
| Session 1 | Checkout validation         | Passed                   |
| Session 1 | Mobile viewport basic check | Passed                   |
| Session 1 | DevTools Console check      | No critical errors found |

## QA Conclusion

No confirmed bugs were found during the first testing session.

The tested critical user flow worked as expected:

Home page → Product search → Product details → Add to cart → Cart → Checkout.

Further testing may include cross-browser testing, deeper mobile viewport testing, accessibility checks and exploratory testing.
