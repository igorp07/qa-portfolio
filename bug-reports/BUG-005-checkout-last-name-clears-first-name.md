# BUG-005 — Last Name input clears First Name field on checkout

**Environment:** Web | Chrome | Windows

**Precondition:** User is logged in and has at least one product in the cart

## Steps to Reproduce

1. Acess the Saude Demo website
2. Log in with a valid user
3. Add any product to the cart
4. Proceed to checkout
5. In the "First Name" field, type a multi-character name (e.g., "Marcelo")
6. 6. Click into the "Last Name" field and start typing a last name (e.g., "Soares")
7. Observe the "First Name" field while typing in "Last Name"

## Actual Result
While typing in the "Last Name" field, the content in the "First Name" field is cleared and replaced by the last typed character (only one character remains).

## Expected Result
Typing in the "Last Name" field should not modify the value entered in the "First Name" field. Each field should keep its own input value independently.

## Severity
High

## Priority
High

## Notes
- Issue appears to behave like both fields are sharing the same input state or handler.
- Reproduced by typing multiple characters in "Last Name" and observing that only the most recent character remains in "First Name".
