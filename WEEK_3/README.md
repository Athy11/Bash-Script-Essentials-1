# BASIC CONTROL FLOW
The Basic Control Flow determines how a program moves from one instruction to the next based on statements, conditions, and loops. 

## CONDITIONAL STATEMENTS
Conditional statements allow executing commands based on certain conditions.

### COMPARISON OPERATORS
| Operator | Description |
| ----------- | ----------- |
| -eq | Equal to ([ x -eq y ]) |
| -ne | Not equal to ([ x -ne y ]) |
| -gt | Greater than ([ x -gt y ]) |
| -ge | Greater than or equal to ([ x -ge y ]) |
| -lt | Less than ([ x -lt y ]) |
| -le | Less than or equal to ([ x -le y ]) |

### IF-ELIF-ELSE STATEMENT
This is used to check multiple conditions while applying the conditional operators.
```bash
#!/bin/bash

echo "Enter a number: "
read num

if [ $num -gt 0 ]; then
    echo "The number is positive."
elif [ $num -lt 0 ]; then
    echo "The number is negative."
else
    echo "The number is zero."
fi
```

## CASE STATEMENT
This is used for multiple checking of values and is much preferred than If-Else Statement as it is easier to read.
```bash
#!/bin/bash

echo "Enter a fruit name (apple, banana, orange):"
read fruit

case $fruit in
    apple )
        echo "You selected an Apple.";;
    banana)
        echo "You selected a Banana.";;
    orange)
        echo "You selected an Orange.";;
    *)
        echo "Invalid selection.";;
esac
```

## LOOPS
Loops are control flow structures that allow repeating a block of code multiple times based on conditions.

### FOR LOOP
This loop is used to iterate over a sequence or range.

#### C-STYLE FOR LOOP
This syntax is similar to the for loop in C, Java, and other languages. It consists of three parts:
- Initialization (i=0): Set the starting value.
- Condition (i < n): Loop runs while this condition is true.
- Increment/Decrement (i++): Updates the variable

```bash
#!/bin/bash

echo "Countdown from 5 to 1"

for ((i = 5; i >= 1; i--))
do
    echo "Countdown: $i"
done
```
#### FOR-IN LOOP

### WHILE LOOP
The while loop executes a block of code as long as a specified condition is true.

### UNTIL LOOP
The until loop executes a block of code until a specified condition becomes true (opposite of while).



