# Unexpected String Concatenation in JavaScript
This example demonstrates a common JavaScript pitfall: unexpected string concatenation due to type coercion.  When using the '+' operator with a mix of numbers and strings, JavaScript will implicitly convert the number to a string and perform concatenation instead of addition.

## Bug Report
The `foo` function is intended to add two numbers. However, when one of the arguments is a string, it results in string concatenation rather than numerical addition.

## Solution
The solution involves explicitly converting both arguments to numbers before performing the addition using `parseInt()` or `Number()`, ensuring the correct numerical operation is executed.