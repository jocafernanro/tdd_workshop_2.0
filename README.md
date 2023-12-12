# tdd_workshop_2.0
A simple TDD workshop with exercises. 2.0 version (1.0 version: https://github.com/jocafernanro/tdd_workshop)

# Calculator TDD exercise
Implement a basic calculator following the TDD principles and good practices.

## Functionalities
- Addition (+): 
    - Sum two natural numbers
    - No negative values
    - Just numbers. Don't accept any other type of data
- Subtraction (-): 
    - Subtract one natural number from another.
    - No negative results (ensure first number is always greater or equal to the second).
    - Accept only numbers, no other data types.
- Multiplication (*):
    - Multiply two natural numbers.
    - No negative values.
    - Accept only numbers, no other data types.
    - Multiplying any number by zero should return zero.
- Division (/):
    - Divide one natural number by another.
    - No negative values.
    - Accept only numbers, no other data types.
    - Division by zero is not allowed and should be handled appropriately.
- Check if a Number is Odd
    - Determine if a given natural number is odd.
    - Accept only natural numbers, no other data types.
    - Negative numbers or zero should not be considered.
- Check if a Number is Even
    - Determine if a given natural number is even.
    - Accept only natural numbers, no other data types.
    - Negative numbers or zero should not be considered.

## Test cases

### Addition
- Sum 4 + 6: Expected result 10.
- Sum 20 + 3: Expected result 23.
- Sum 0 + 7: Expected result 7.
- Sum 0 + 0: Expected result 0.
- Sum with Non-Number (e.g., 'a' + 5): Expected to throw an error.

### Subtraction
- Subtract 5 - 3: Expected result 2.
- Subtract 20 - 7: Expected result 13.
- Subtract 3 - 3: Expected result 0.
- Subtract with Non-Number (e.g., 5 - 'b'): Expected to throw an error.
- Subtract 3 - 5: Expected to handle/throw an error (no negative results).

### Multiplication
- Multiply 4 * 3: Expected result 12.
- Multiply 5 * 10: Expected result 50.
- Multiply 5 * 0: Expected result 0.
- Multiply with Non-Number (e.g., 'a' * 2): Expected to throw an error.
- Multiply 0 * 0: Expected result 0.

### Division
- Divide 6 / 3: Expected result 2.
- Divide 25 / 5: Expected result 5.
- Divide 5 / 0: Expected to throw an error or handle it.
- Divide with Non-Number (e.g., 9 / 'c'): Expected to throw an error.
- Divide 0 / 3: Expected result 0.

### Check if a Number is Odd
- Check Odd for 3: Expected result true.
- Check Odd for 6: Expected result true.
- Check Odd for 4: Expected result false.
- Check Odd for 0: Expected to throw an error or handle it.
- Check Odd with Non-Number (e.g., 'a'): Expected to throw an error.

### Check if a Number is Even
- Check Even for 4: Expected result true.
- Check Even for 8: Expected result true.
- Check Even for 3: Expected result false.
- Check Even for 0: Expected to throw an error or handle it.
- Check Even with Non-Number (e.g., 'b'): Expected to throw an error.

## Commands

Install dependencies:
```npm install```

Run all tests:
```npm run tests```

Run all tests and watch changes:
```npm run tests:watch```