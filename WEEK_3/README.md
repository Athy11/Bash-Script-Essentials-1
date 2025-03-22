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
This loop iterates over lists, filenames, or a predefined range (for item in list).
```bash
#Iterating Over a List of Words
#!/bin/bash
for item in Apple Banana Cherry; do
    echo "Fruit: $item"
done

#Iterating Over a Range
#!/bin/bash
for i in {1..5}; do
    echo "Number: $i"
done

#Iterating Over Files
#!/bin/bash
for file in *.txt; do
    echo "Processing $file"
done
```

### WHILE LOOP
The while loop executes a block of code as long as a specified condition is true.
```bash
#This is while loop with array 
#!/bin/bash

arr=("Apple" "Banana" "Cherry" "Date")
i=0

while [ $i -lt ${#arr[@]} ]
do
    echo "Fruit: ${arr[i]}"
    ((i++))
done

------------
#This is while loop with if-statement
#!/bin/bash
num=0

while [ $num -lt 10 ]
do
    ((num++))

    if [ $num -eq 5 ]; then
        echo "Skipping number 5"
        continue
    fi

    if [ $num -eq 8 ]; then
        echo "Breaking the loop at 8"
        break
    fi

    echo "Number: $num"
done
```

### UNTIL LOOP
The until loop executes a block of code until a specified condition becomes true (opposite of while).
```bash
#This code checks if the password is the same as the declared value and hides the user input.
#!/bin/bash

correct_pass="CNCP"
user_input=""

until [ "$user_input" = "$correct_pass" ]; do
    read -s -p "Enter password: " user_input
    echo  # Move to a new line
done

echo "Access granted!"
```
## LET’S PRACTICE YOUR KNOWLEDGE
Now that you know the Basic Control Flow in Bash, let's challenge your knowledge!
Create a program where the user must guess a random number from 1 to 10 using until loop and if statement.
