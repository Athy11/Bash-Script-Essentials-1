# ASSIGNMENT 3
Now that you know the Basic Control Flow in Bash, let's challenge your knowledge! 

**DETAILS:**
Create a program where the user must guess a random number from 1 to 10 using until loop and if statement.

## SAMPLE CODE
**STEP 1:**
Create a file where you will write the code.
```bash
vim week3.sh
```

**STEP 2:**
Add the shebang (#!) to indicate which interpreter we will use (bash).
```bash
#!/bin/bash
```

**STEP 3:**
Write your simple guessing game script/code, it can look similar to this.
```bash
#!/bin/bash

target=$(( RANDOM % 10 + 1 ))
guess=0

until [[ "$guess" -eq "$target" ]]; do
        echo Guess a number from 1-10:
        read guess
        [[ "$guess" -lt "$target" ]] && echo too low
        [[ "$guess" -gt "$target" ]] && echo too high
done

echo "Congrats! The number was indeed $target"

```
> Save the file by typing **`:w`** or **`:wq`**.

**STEP 4:**
Change the permission
```bash
chmod u+x week3.sh
```
**STEP 5:**
Run your script.
```bash
./week3.sh
```
