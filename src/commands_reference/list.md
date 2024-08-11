# List

List is way to use plural value together.
In this chapter, Let you know how to processing list in Stack.

## Get
This command is to get list value of specified index.

**Example**:
In this code, print the "Hello, world!" message.
```stack-lang
[(a) (b) (c)] 1 get
```

**Result**:
```stack-repl
Stack〔  〕 ←  [(a) (b) (c)]
Stack〔  〕 ←  (a)
Stack〔 (a) 〕 ←  (b)
Stack〔 (a) | (b) 〕 ←  (c)
Stack〔 (a) | (b) | (c) 〕
Stack〔 [(a) (b) (c)] 〕 ←  1
Stack〔 [(a) (b) (c)] | 1 〕 ←  get
Stack〔 (b) 〕
```

## Set
This command is to sex list value of specified index.

**Example**:
In this code, print the "Hello, world!" message.
```stack-lang
[(a) (b) (c)] 1 (B) set
```

**Result**:
```stack-repl
Stack〔  〕 ←  [(a) (b) (c)]
Stack〔  〕 ←  (a)
Stack〔 (a) 〕 ←  (b)
Stack〔 (a) | (b) 〕 ←  (c)
Stack〔 (a) | (b) | (c) 〕
Stack〔 [(a) (b) (c)] 〕 ←  1
Stack〔 [(a) (b) (c)] | 1 〕 ←  (B)
Stack〔 [(a) (b) (c)] | 1 | (B) 〕 ←  set
Stack〔 [(a) (B) (c)] 〕
```
