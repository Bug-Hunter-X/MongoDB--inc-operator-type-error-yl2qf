# MongoDB $inc Operator Type Error
This example demonstrates a common error when using the `$inc` operator in MongoDB update queries.  The `$inc` operator is used to increment a numeric field by a specified value.  However, if a non-numeric value (e.g., a string) is provided, it will result in an unexpected outcome, potentially silently failing or causing a type error.  The provided solution showcases the correct usage and emphasizes the importance of using numbers with the `$inc` operator.

## Bug
The bug involves passing a string value ('1') to the `$inc` operator instead of a number (1).  This incorrect usage can lead to unexpected behavior, as the MongoDB driver may not handle the type mismatch properly.

## Solution
The correct usage of the `$inc` operator requires passing a numeric value as the increment.  Replacing the string '1' with the number 1 will resolve the issue. 