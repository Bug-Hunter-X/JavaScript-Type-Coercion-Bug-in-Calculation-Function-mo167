# JavaScript Type Coercion Bug

This repository demonstrates a potential bug in JavaScript related to type coercion within a simple calculation function. The `calculate` function performs addition or subtraction based on the provided operation, but it does not explicitly handle non-numeric inputs. This can lead to unexpected results.

## Bug Description

The core issue lies in the lack of input validation.  If the function receives non-numeric values for `a` or `b`, JavaScript's type coercion will attempt to convert them to numbers, potentially resulting in incorrect calculations or unexpected behavior.

## Solution

The solution involves adding input validation to ensure that `a` and `b` are numbers before performing the calculations.  This can be achieved using `typeof` or `isNaN` checks.