# BUG-003 — Checkout allows purchase with empty cart

**Environment:** Web | Chrome | Windows

**Precondition:** User is logged in

## Steps to Reproduce

1. Log in to the Sauce Demo website
2. Open the cart page
3. Proceed to checkout
4. Fill in First Name, Last Name, and Postal Code with valid values
5. Click on the "Continue" button
6. Complete the checkout process

## Actual Result
The system allows the user to proceed through checkout and complete the purchase even when the cart is empty

## Expected Result
The system should prevent the user from proceeding to checkout and display a message indicating that at least one product must be added to the cart before completing a purchase.

## Severity
High

## Priority
High

## Notes
- Issue occurs even when no products are added to the cart.
- Checkout flow does not validate cart state before allowing purchase completion.
