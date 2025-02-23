# MongoDB $inc Operator Error
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The error occurs when providing a string value to the `$inc` operator instead of a number. This results in the `count` field not being incremented as expected.

## Bug Description
The code attempts to increment the `count` field in a MongoDB document using the `$inc` operator.  However, the value passed to `$inc` is a string ("1"), instead of a number (1).  This leads to an unexpected result, where the field is not incremented correctly.

## Solution
The solution involves correcting the value passed to the `$inc` operator to a numeric value.