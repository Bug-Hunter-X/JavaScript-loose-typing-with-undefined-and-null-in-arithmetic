# JavaScript Loose Typing Bug

This example demonstrates a common issue in JavaScript related to loose typing when performing arithmetic operations involving `null` and `undefined`.

## The Bug

The core problem is the inconsistent behavior of the `+` operator when one operand is `null` and the other is a number, versus when one operand is `undefined` and the other is a number.

- Adding `undefined` to a number results in `NaN` (Not a Number).
- Adding `null` to a number results in the number (as null is coerced to 0).

This inconsistency can cause unexpected behavior in your code if not handled carefully.

## The Solution

The best approach is to always explicitly check for `null` and `undefined` values before performing arithmetic and handle them appropriately, perhaps by using a default value or throwing an error.
