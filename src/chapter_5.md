# Variable

Stack properly has variable.
You can use `var` command to define variable.

Enter below program to use variable at Stack REPL.
```
(Alice) (name) var
name print
```

Then, output inside stack view at Stack REPL.
```
Stack〔  〕 ←  (Alice)
Stack〔 (Alice) 〕 ←  (name)
Stack〔 (Alice) | (name) 〕 ←  var
Variables {
 name: (Alice)
}
Stack〔  〕 ←  name
Stack〔 (Alice) 〕 ←  print
[Output]: Alice
```
Great! You saved data in the `name` variable.
The variables are suitable for medium to long term data storage separately from the stack.