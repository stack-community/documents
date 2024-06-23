# Control

Any programming language needs control syntax. 
In this chapter, Explain control syntax such as `if`, `while` etc of Stack.

## If

**Example**:  
In this code, judgement which even or odd is 5987.
```stack-lang
(Even print) 
(Odd print)
5987 2 mod 0 equal if
```

**Result**:  
```stack-repl
Stack〔  〕 ←  (Even print)
Stack〔 (Even print) 〕 ←  (Odd print)
Stack〔 (Even print) | (Odd print) 〕 ←  5987
Stack〔 (Even print) | (Odd print) | 5987 〕 ←  2
Stack〔 (Even print) | (Odd print) | 5987 | 2 〕 ←  mod
Stack〔 (Even print) | (Odd print) | 1 〕 ←  0
Stack〔 (Even print) | (Odd print) | 1 | 0 〕 ←  equal
Stack〔 (Even print) | (Odd print) | false 〕 ←  if
Stack〔  〕 ←  Odd
Stack〔 (Odd) 〕 ←  print
[Output]: Odd
```
