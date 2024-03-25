# Calculate

Let's calculate mathematical formula by Stack.
Enter below program to simply calculate at Stack REPL.

```stack
1 2 add
```

Then, output inside stack view at Stack REPL.

```stack
Stack〔  〕 ←  1
Stack〔 1 〕 ←  2
Stack〔 1 | 2 〕 ←  add
Stack〔 3 〕
```

Great! You can calculate by Stack.

> `add` is the command of addition the number.

2nd, more difficult formula. 
Stack REPL can input multi-lines program.

```stack
2 3 4 add add 5 sub 
4 mul 3 div round
```

Correct to processing difficult formula!
```
Stack〔  〕 ←  2
Stack〔 2 〕 ←  3
Stack〔 2 | 3 〕 ←  4
Stack〔 2 | 3 | 4 〕 ←  add
Stack〔 2 | 7 〕 ←  add
Stack〔 9 〕 ←  5
Stack〔 9 | 5 〕 ←  sub
Stack〔 4 〕 ←  4
Stack〔 4 | 4 〕 ←  mul
Stack〔 16 〕 ←  3
Stack〔 16 | 3 〕 ←  div
Stack〔 5.333333333333333 〕 ←  round
Stack〔 5 〕
```

> `sub` is the command of subtraction the number.

> `mul` is the command of multiplication the number.

> `div` is the command of division the number.

> `round` is the command of rounding off the number.

Stack is good at processing mathematical formula too.