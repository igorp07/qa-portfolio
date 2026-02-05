# BUG-001 — Checkout allows purchase without first name and last name

**Environment:** Web | Chrome | Windows

**Precondition:** Product added to cart

## Steps to Reproduce
1. Access the Sauce Demo website
2. Log in with a valid user
3. Add the product "Sauce Labs Bike Light" to the cart
4. Open the cart and proceed to checkout
5. Leave the First Name and Last Name fields empty and fill the Postal Code with a single space (" ")
6. Click on the "Continue" button

## Actual Result
The system allows the user to proceed with the checkout even when the First Name and Last Name fields are empty and the Postal Code contains only a space.

## Expected Result
The system should prevent the user from proceeding with the checkout and display a validation message indicating that First Name, Last Name, and Postal Code are required and must contain valid values.

## Severity
High

## Priority
High

## Notes
- Issue reproduces only with specific products, such as "Sauce Labs Bike Light".
- Validation behavior differs when other products are used.
