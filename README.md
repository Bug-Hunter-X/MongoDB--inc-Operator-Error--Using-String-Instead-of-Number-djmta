# MongoDB $inc Operator Error: Using String Instead of Number

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment a numeric field by a specified value.  However, if a string is provided as the increment value, the operation will fail unexpectedly instead of throwing an error.

## Bug
The bug is in the use of the `$inc` operator in the `updateOne` method in a MongoDB query. The increment value is passed as a string rather than a number. This leads to the field not being incremented correctly.

## Solution
The solution is to ensure that the increment value passed to the `$inc` operator is a number.  The corrected code uses a numeric value for the increment, ensuring that the field is updated as expected.
