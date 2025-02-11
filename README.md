# JavaScript Bug: Null Input Handling in Addition Function

This repository demonstrates a common JavaScript bug related to null input handling in an addition function. The function `foo` is designed to add two numbers, but it unexpectedly returns `null` if either input is `null`. This behavior might not be intuitive or desirable in all cases.

## Bug Description

The `foo` function uses a strict equality check (`===`) to compare inputs with `null`.  While this correctly identifies null values, it leads to premature null return, regardless of whether the other argument is a valid number.  A more robust solution is needed to handle null inputs gracefully.

## Solution

The solution implements improved null handling using loose equality (`==`) or by providing default values for null inputs, enabling the function to proceed with calculations even when one input is `null`.