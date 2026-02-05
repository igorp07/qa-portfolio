# CT-003 — Validate independent behavior of First Name and Last Name fields

**Precondition:** User is logged in and has at least one product in the cart

## Test Steps

1. Access the Sauce Demo website
2. Log in with a valid user
3. Add any product to the cart
4. Proceed to checkout
5. Enter a multi-character value in the "First Name" field (e.g., "Marcelo")
6. Click on the "Last Name" field
7. Type a multi-character value in the "Last Name" field (e.g., "Soares")
8. Observe the value in the "First Name" field while typing in "Last Name"

## Expected Result
Typing in the "Last Name" field should not modify or clear the value entered in the "First Name" field. Each input field must maintain its value independently.

## Test Status
Fail
