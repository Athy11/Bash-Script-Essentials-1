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



