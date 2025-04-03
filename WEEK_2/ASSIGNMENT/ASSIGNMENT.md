# ASSIGNMENT 2
Now that you’ve learned how to do Input/Output Redirection and create variables, it is now the time to use what you’ve learned!

**DETAILS:**
You can create a simple calculator or any simple program that utilizes Input or Output Redirection.

## SAMPLE CODE
**STEP 1:**
Create a file where you will write the code.
```bash
vim week2.sh
```

**STEP 2:**
Add the shebang (#!) to indicate which interpreter we will use (bash).
```bash
#!/bin/bash
```

**STEP 3:**
Write your simple calculator script/code, it can look similar to this.
```bash
#!/bin/bash
echo Enter two numbers:
read num1 num2

sum = $($num1 + $num2)
echo $sum
```
If you want to try the advanced version of this, here's how:
```bash
#!/bin/bash
echo Enter two numbers:
read num1 num2
echo "Enter operator to use (+, -, /, *):"
read op

result=$(awk "BEGIN {print $num1 $op $num2}")

echo "Result: $result"
```
> Save the file by typing **`:w`** or **`:wq`**.

**STEP 4:**
Change the permission
```bash
chmod u+x week2.sh
```
**STEP 5:**
Run your script.
```bash
./week2.sh
```


