# Control

Any programming language needs control syntax. 
In this chapter, Explain control syntax such as `if`, `while` etc of Stack.

## If
If is important way to branch program execution.

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

## While
While is usual way to loop program.

**Example**:  
```stack-lang
1 (i) var 
(
    i println
    i 1 add (i) var
) (i 2 less) while
(Finished) println
```

**Result**:  
```stack-repl
Stack〔  〕 ←  1
Stack〔 1 〕 ←  (i)
Stack〔 1 | (i) 〕 ←  var
Variables {
 i: 1
}
Stack〔  〕 ←  ( i println i 1 add (i) var )
Stack〔 ( i println i 1 add (i) var ) 〕 ←  (i 2 less)
Stack〔 ( i println i 1 add (i) var ) | (i 2 less) 〕 ←  while
Stack〔  〕 ←  i
Stack〔 1 〕 ←  2
Stack〔 1 | 2 〕 ←  less
Stack〔 true 〕
Stack〔  〕 ←  i
Stack〔 1 〕 ←  println
[Output]: 1
Stack〔  〕 ←  i
Stack〔 1 〕 ←  1
Stack〔 1 | 1 〕 ←  add
Stack〔 2 〕 ←  (i)
Stack〔 2 | (i) 〕 ←  var
Variables {
 i: 2
}
Stack〔  〕
Stack〔  〕 ←  i
Stack〔 2 〕 ←  2
Stack〔 2 | 2 〕 ←  less
Stack〔 false 〕
Stack〔  〕 ←  (Finished)
Stack〔 (Finished) 〕 ←  println
[Output]: Finished
```
