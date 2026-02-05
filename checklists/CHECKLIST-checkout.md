# Checkout Test Checklist

This checklist covers essential validations and behaviors that should be verified during the checkout process.

---

## Cart Validation
- [ ] Checkout is blocked when the cart is empty
- [ ] User cannot proceed to checkout without at least one product in the cart
- [ ] Cart accurately reflects added and removed products

---

## Required Fields
- [ ] First Name field is required
- [ ] Last Name field is required
- [ ] Postal Code field is required
- [ ] Fields do not accept empty or whitespace-only values

---

## Input Behavior
- [ ] First Name and Last Name fields behave independently
- [ ] Typing in one field does not affect other fields
- [ ] Fields accept multi-character input correctly

---

## Navigation and State
- [ ] Validation is re-applied after navigating back and forth between steps
- [ ] Form state does not persist incorrectly after navigation
- [ ] Checkout flow maintains consistent validation behavior

---

## Error Handling
- [ ] Clear and informative error messages are displayed for invalid input
- [ ] Errors are shown near the corresponding fields
- [ ] User can correct errors and proceed successfully

---

## Successful Checkout
- [ ] User can complete checkout with valid data and at least one product in the cart
- [ ] Checkout completes only once all validations pass
