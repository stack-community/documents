# Calculation
Stack's expression is Reverse Polish Notation (RPN). That's result of stack oriented approach.

RPN is a mathematical notation wherein every operator follows all of its operands. It is also known as postfix notation. In contrast to the more common infix notation, where operators are placed between operands (e.g., `3 + 4`), RPN eliminates the need for parentheses to define operation order.

## Advantages of RPN

- **No Need for Parentheses**: RPN eliminates the need for parentheses that are required in Usual notation to dictate the order of operations.
- **Efficient for Computers**: RPN is easier to implement on computers as it suits stack-based calculations.
- **Reduces Errors**: Human errors related to misplacing parentheses are reduced.


## Addition
In Stack, to add two numbers, you would write the operands first, followed by the operator.

> the "Usual" is based on Python's syntax 

**Example**:  
Usual: `3 + 4`  
Stack: `3 4 add`

**Result**:  
```stack-repl
Stack〔  〕 ←  3
Stack〔 3 〕 ←  4
Stack〔 3 | 4 〕 ←  add
Stack〔 7 〕
```
## Subtraction
For subtraction, the Stack format follows the same pattern: operands first, then the operator.

**Example**:  
Usual: `7 - 2`  
Stack: `7 2 sub`

**Result**:  
```stack-repl
Stack〔  〕 ←  7
Stack〔 7 〕 ←  2
Stack〔 7 | 2 〕 ←  sub
Stack〔 5 〕
```

## Multiplication
Multiplication in Stack is handled similarly.

**Example**:  
Usual: `5 * 6`  
Stack: `5 6 mul`

**Result**:  
```stack-repl
Stack〔  〕 ←  5
Stack〔 5 〕 ←  6
Stack〔 5 | 6 〕 ←  mul
Stack〔 30 〕
```

## Division
Division follows the same postfix notation rules.

**Example**:  
Usual: `8 / 4`  
Stack: `8 4 div`

**Result**:  
```stack-repl
Stack〔  〕 ←  8
Stack〔 8 〕 ←  4
Stack〔 8 | 4 〕 ←  div
Stack〔 2 〕
```

## Modulo
If we want modulo of division, we can use `mod` command.
**Example**:  
Usual: `90 % 7 `  
Stack: `90 7 mod`

**Result**:  
```stack-repl
Stack〔  〕 ←  90
Stack〔 90 〕 ←  7
Stack〔 90 | 7 〕 ←  mod
Stack〔 6 〕
```

## Power
Sometimes, we have to powering number. If so case, we can use `pow` command. 

**Example**:  
Usual: `2 ** 10`  
Stack: `2 10 pow`

**Result**:  
```stack-repl
Stack〔  〕 ←  2
Stack〔 2 〕 ←  10
Stack〔 2 | 10 〕 ←  pow
Stack〔 1024 〕
```


## Rounding off
Disision isn't always divisible, It need rounding off.
**Example**:  
Usual: `round(22 / 7)`  
Stack: `22 7 div round`

**Result**:  
```stack-repl
Stack〔  〕 ←  22
Stack〔 22 〕 ←  7
Stack〔 22 | 7 〕 ←  div
Stack〔 3.142857142857143 〕 ←  round
Stack〔 3 〕
```

## Combining Operations

Stack can also handle more complex expressions by maintaining the order of operations through its postfix structure.

**Example 1**:  
Usual: `(3 + 4) * 2`  
Stack: `3 4 add 2 mul`

**Result 1**:  
```stack-repl
Stack〔  〕 ←  3
Stack〔 3 〕 ←  4
Stack〔 3 | 4 〕 ←  add
Stack〔 7 〕 ←  2
Stack〔 7 | 2 〕 ←  mul
Stack〔 14 〕
```
**Example 2**:  
Usual: `5 + ((1 + 2) * 4) - 3`  
Stack: `5 1 2 add 4 mul add 3 sub`

**Result 2**:  
```stack-repl
Stack〔  〕 ←  5
Stack〔 5 〕 ←  1
Stack〔 5 | 1 〕 ←  2
Stack〔 5 | 1 | 2 〕 ←  add
Stack〔 5 | 3 〕 ←  4
Stack〔 5 | 3 | 4 〕 ←  mul
Stack〔 5 | 12 〕 ←  add
Stack〔 17 〕 ←  3
Stack〔 17 | 3 〕 ←  sub
Stack〔 14 〕
```