# MongoDB $inc Operator Error

This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries.  The `$inc` operator is used to increment a numerical field by a specified value. However, providing a string value instead of a number will result in an incorrect update or an error.

## Bug
The `bug.js` file contains code that incorrectly uses the `$inc` operator, supplying a string value ('1') instead of a numerical value (1). This results in the `age` field not being incremented correctly.

## Solution
The `bugSolution.js` file shows the correct usage, using a numerical value to increment the field.

## How to reproduce
1. Ensure you have MongoDB installed and running.
2. Create a collection named `myCollection`.
3. Insert a document with a field `age`. 
4. Run the code in `bug.js` to see the error or unexpected result.
5. Run the code in `bugSolution.js` to see the correct implementation.