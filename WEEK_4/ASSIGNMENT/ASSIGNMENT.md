# ASSIGNMENT 4
Now that you learned how functions and modular programming in Bash works. It's time to practice your skills! Enhance the simple calculator by adding case or if-statement and loops!

**DETAILS:**
Write a script that lets the user choose an operation (Addition, Subtraction, Multiplication, Division) and performs the calculation by calling the function based on the user's choice.

## SAMPLE CODE
**STEP 1:**
Create a file where you will write the main code/script.
```bash
vim week4.sh
```

**STEP 2:**
Add the shebang (#!) to indicate which interpreter we will use (bash).
```bash
#!/bin/bash
```

**STEP 3:**
Create a different file where you will write the simple function of a calculator, it can look similar to this. Name teh file as **`operation.sh`**. 
```bash
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
> Save the file by typing **`:w`** or **`:wq`**.

**STEP 4**
Create a file where you will ask the user to input two numbers and the operator to use. Call the **`operation.sh`** file to compute.
> Save the file by typing **`:w`** or **`:wq`**.

**STEP 5:**
Change the permission.
```bash
chmod u+x week4.sh
```
**STEP 6:**
Run your script by calling the main file.
```bash
./week4.sh
```
