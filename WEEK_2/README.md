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

```bash
#!/bin/bash
is_valid=1
if [ "$is_valid” -eq 1 ]; then
  echo TRUE
else
  echo FALSE
fi

Output: TRUE
```
## User Input in Bash
To take user input in Bash, we use the read command.
```bash
#!/bin/bash
echo "Are you enjoying this course?"
read answer

Output: 
Are you enjoying this course?
Yes!
```
### Let’s try taking multiple inputs this time!
```bash
#!/bin/bash
echo Enter your first and last name:
read fname lname 
echo Your full name is $fname $lname

Output:
Enter your first and last name:
Liza Soberano
You full name is Liza Soberano
```

### Let’s try hidden inputs! 
This is used if you’re dealing with passwords. The entered value will not be visible as you type.
```bash
#!/bin/bash
echo Enter your password:
read -s password
echo Password received!

Output:
Enter your password:
Password received!
```
## OUTPUT REDIRECTION
It redirects command output from the terminal to a file.
| Symbol | Description |
| ----------- | ----------- |
| > | Overwrites the file with new output |
| >> | Appends output to the file without overwriting |

## INPUT REDIRECTION
It allows a command or script to read data from a file instead of manual user input.
| Symbol | Description |
| ----------- | ----------- |
| < | Reads input from a file instead of standard input. |
| << | Used for multi-line input redirection |

## LET’S PRACTICE YOUR KNOWLEDGE
Now that you’ve learned how to do Input/Output Redirection and create variables, it is now the time to use what you’ve learned!

You can create a simple calculator or any simple program that utilizes Input or Output Redirection.  







