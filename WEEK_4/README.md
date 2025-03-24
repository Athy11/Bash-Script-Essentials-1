# FUNCTIONS AND MODULAR PROGRAMMING
Functions in Bash allow you to write reusable blocks of code that can be called multiple times within a script, improving organization and reducing redundancy. Modular programming takes this further by splitting code into separate files (modules) that can be sourced when needed, making scripts more maintainable and scalable.

## FUNCTION IN BASH
A function in Bash is a named block of code that performs a specific task and can be executed whenever needed. Using functions helps break down complex scripts into smaller, manageable parts, making the script easier to read and debug. In creating a function, you can do it with or without the keyword **function**. You can also pass arguments using special variables ($1, $2...).

### WITH FUNCTION KEYWORD
```bash
function greet() {
    echo "Welcome to CNCP, $1!"
}

greet "Cutie"
```

### WITHOUT FUNCTION KEYWORD
```bash
greet() {
    echo "Welcome to CNCP, $1!"
}

greet "Cutie"
```

## MODULAR PROGRAMMING IN BASH
It involves organizing reusable functions into separate files (modules) and including them in scripts as needed. This approach enhances code reusability, improves maintainability, and keeps scripts clean. Instead of rewriting common functions, we store them in a separate file and access them.

```bash
#This file is named simple_calc.sh
#!/bin/bash

add() {
    echo $(( $1 + $2 ))
}

subtract() {
    echo $(( $1 - $2 ))
}

multiply() {
    echo $(( $1 * $2 ))
}

divide() {
    echo $(( $1 / $2 ))
}
```
```bash
#This is the file where we will access the simple_calc.sh

#!/bin/bash
# Import functions from simple_calc.sh
source simple_calc.sh

result=$(add 3 7)
echo "SUM: $result"

result=$(subtract 42 41)
echo "DIFFERENCE: $result"

result=$(multiply 5 5)
echo "PRODUCT: $result"

result=$(divide 50 5)
echo "QUOTIENT: $result"
```

## LET’S PRACTICE YOUR KNOWLEDGE
Now that you learned how functions and modular programming in Bash works. It's time to practice your skills! Enhance the simple calculator by adding case or if-statement and loops! 

Write a script that lets the user choose an operation (Addition, Subtraction, Multiplication, Division) and performs the calculation by calling the function based on the user's choice.
