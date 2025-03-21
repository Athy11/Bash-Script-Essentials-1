# VARIABLES AND I/O OPERATIONS
In Bash Scripting, it does not have the traditional data types like in other programming languages that have integer, string, float, and boolean. Instead, all variables in Bash are treated as strings by default, but it can perform operations on numbers and handle different types of values. 

## String in Bash 
In Bash, all variables are treated as a string, it is the default data type. You can write the value inside a double quotation mark or without. There should be no spacing after the equal sign (=), because the value will not be read. 

```bash
#!/bin/bash
msg1=Welcome to
org=”CNCP!”
echo $msg1 $org
Output: Welcome to CNCP!
```
## Integer in Bash 
In Bash, even if all variables are treated as a string we can still perform arithmetic operations like addition (+), subtraction (-), multiplication (*), division (/), modulus (%), exponentiation (**), increment (++), and decrement (--). In performing these operations it must be enclosed with double parenthesis.

```bash
#!/bin/bash
num1=10
num2=5
sum=$((num1 + num2))  
echo "Sum: $sum"
Output:Sum: 15
```
## Boolean in Bash
In Bash, it does not have a built-in Boolean type, but it uses 0 for false and 1 for true. 
Here are the Comparison Operators used for integer values inside if-statements.
| Operator | Description |
| ----------- | ----------- |
| Header | Title |
| -eq | Equal to (==) |
| -ne | Not equal to (!=) |



