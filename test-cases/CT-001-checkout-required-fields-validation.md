# CT-001 — Validate required fields on checkout
**Precondition:** User is logged in and has a product in the cart
## Test Steps
1. Access the checkout page
2. Verify that the First Name, Last Name, and Postal Code fields are displayed
3. Leave the First Name and Last Name fields empty
4. Enter a single space (" ") in the Postal Code field
5. Click on the "Continue" button

## Expected Result
The system should prevent the user from proceeding and display validation messages indicating that First Name, Last Name, and Postal Code are required and must contain valid values.
## Test Status
Fail
