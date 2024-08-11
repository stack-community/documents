# List

List is way to use plural value together.
In this chapter, Let you know how to processing list in Stack.

## Get
This command is to get list value of specified index.

**Example**:
In this code, print the "Hello, world!" message.
```stack-lang
[1 2 3] 1 get
```

**Result**:
```stack-repl
Stack〔  〕 ←  [1 2 3]
Stack〔  〕 ←  1
Stack〔 1 〕 ←  2
Stack〔 1 | 2 〕 ←  3
Stack〔 1 | 2 | 3 〕
Stack〔 [1 2 3] 〕 ←  1
Stack〔 [1 2 3] | 1 〕 ←  get
Stack〔 2 〕
```
