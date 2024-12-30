# MongoDB $inc Operator Error with Non-Numeric Value
This repository demonstrates an example of a common error encountered when using the `$inc` operator in MongoDB updates. The error arises when attempting to increment a field with a non-numeric value.

## Bug Description
The `$inc` operator in MongoDB is designed to increment a numeric field by a specified value.  However, if you provide a non-numeric value (like a string or object), the update operation will fail and throw an error.

## Bug Reproduction
The `bug.js` file contains code that reproduces this error.  Running the code will cause the MongoDB update operation to fail.

## Bug Solution
The `bugSolution.js` file demonstrates the correct way to use the `$inc` operator.  The solution involves ensuring that you are using a numeric value as the increment amount.