# Control

Any programming language needs control syntax. 
In this chapter, Explain control syntax such as `if`, `while` etc of Stack.

## If

**Example 1**:  
In this code, judgement which even or odd is 5987.
```stack-lang
(Even print) 
(Odd print)
5987 2 mod 0 equal if
```

**Result 1**:  
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

**Example 2**:  
It needs otherwise, judgement which even or odd is 8762.
```stack-lang
(Even print) 
(Odd print)
8762 2 mod 0 equal if
```

**Result 2**:  
```stack-repl
Stack〔  〕 ←  (Even print)
Stack〔 (Even print) 〕 ←  (Odd print)
Stack〔 (Even print) | (Odd print) 〕 ←  8762
Stack〔 (Even print) | (Odd print) | 8762 〕 ←  2
Stack〔 (Even print) | (Odd print) | 8762 | 2 〕 ←  mod
Stack〔 (Even print) | (Odd print) | 0 〕 ←  0
Stack〔 (Even print) | (Odd print) | 0 | 0 〕 ←  equal
Stack〔 (Even print) | (Odd print) | true 〕 ←  if
Stack〔  〕 ←  Even
Stack〔 (Even) 〕 ←  print
[Output]: Even
```
