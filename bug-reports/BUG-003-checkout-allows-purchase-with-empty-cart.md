# BUG-003 — Checkout allows purchase with empty cart

**Environment:** Web | Chrome | Windows

**Precondition:** User is logged in

## Steps to Reproduce

1. Log in to the Sauce Demo website
2. Add any product to the cart
3. Open the cart
4. Remove the product from the cart
5. Proceed to checkout
6. Fill in First Name, Last Name, and Postal Code with valid values
7. Click on the "Continue" button
8. Complete the checkout process

## Notes
- Issue reproduces regardless of the product added to the cart.
- Checkout flow allows order completion after all products are removed.
- This behavior may result in invalid orders and inconsistent backend data.
