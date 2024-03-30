# Conditional branch

Stack has function of conditional branch.
You can use `if` command to conditional branch.

Enter below program to use variable at Stack REPL.
```
5 (n) var
((It's even) print)
((It's odd) print)
n 2 mod 0 equal if
```

Then, output inside stack view at Stack REPL.
```
Stack〔  〕 ←  5
Stack〔 5 〕 ←  (n)
Stack〔 5 | (n) 〕 ←  var
Variables {
 n: 5
}
Stack〔  〕 ←  ((It's even) print)
Stack〔 ((It's even) print) 〕 ←  ((It's odd) print)
Stack〔 ((It's even) print) | ((It's odd) print) 〕 ←  n
Stack〔 ((It's even) print) | ((It's odd) print) | 5 〕 ←  2
Stack〔 ((It's even) print) | ((It's odd) print) | 5 | 2 〕 ←  mod
Stack〔 ((It's even) print) | ((It's odd) print) | 1 〕 ←  0
Stack〔 ((It's even) print) | ((It's odd) print) | 1 | 0 〕 ←  equal
Stack〔 ((It's even) print) | ((It's odd) print) | false 〕 ←  if
Stack〔  〕 ←  (It's odd)
Stack〔 (It's odd) 〕 ←  print
[Output]: It's odd
```

Great! You got judge number even or odd by conditional branch.
That's important command as control structure.

> Change `n` variable and recheck the result.