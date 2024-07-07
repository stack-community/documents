# Input/Output

I/O is nessesaly thing in any applications.
In this chapter, Let you know how to use I/O in Stack.

## Print
print is common thing in standard outputs. 

**Example**:  
In this code, print the "Hello, world!" message.
```stack-lang
(Hello, world!) print
```

**Result**:  
```stack-repl
Stack〔  〕 ←  (Hello, world!)
Stack〔 (Hello, world!) 〕 ←  print
[Output]: Hello, world!
```

## PrintLn
println is like print.
differnnt point is just with line feed.
**Example**:  
In this code, print the "Hello, world!" message.
```stack-lang
(Hello, world!) println
```

**Result**:  
```stack-repl
Stack〔  〕 ←  (Hello, world!)
Stack〔 (Hello, world!) 〕 ←  println
[Output]: Hello, world!
```

## Input
input is enter from user keyboard.
**Example**:  
In this code, Ask user name.
```stack-lang
(your name: ) input 
(Welcome, ) swap concat println
```

**Result**:  
```stack-repl
Stack〔  〕 ←  (Hello, world!)
Stack〔  〕 ←  (your name: )
Stack〔 (your name: ) 〕 ←  input
your name: StackStick
Stack〔 (StackStick) 〕 ←  (Welcome, )
Stack〔 (StackStick) | (Welcome, ) 〕 ←  swap
Stack〔 (Welcome, ) | (StackStick) 〕 ←  concat
Stack〔 (Welcome, StackStick) 〕 ←  println
[Output]: Welcome, StackStick
```