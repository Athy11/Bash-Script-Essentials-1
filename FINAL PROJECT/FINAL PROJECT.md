## FINAL PROJECT FOR BASH SCRIPT
**DETAILS:**
Write a Bash Script that allows users to input student names and test scores wherein it calculates their average score, and assigns a letter grade based on predefined grading criteria. This final project uses basic control flow, functions, loops, and conditionals that are shared with you throughout this course.

### CONCEPTS TO CONSIDER
| Feature | Description |
| ----------- | ----------- |
| Functions | Used to modularize the logic for grade calculation. |
| Loops  | Used to iterate through multiple students. |
| Conditional Statements | Used to determine the student's letter grade. |
| User Input | Allows dynamic data entry from the user.

### PROGRAM DETAILS GUIDE
**Step 1:** Ask for the Number of Students
The script prompts the user to enter the number of students.

A for loop is used to process each student one by one.

**Step 2:** Input Student Details
- The user is asked to enter the student's name.
- The user is then prompted to enter three test scores.

**Step 3:** Calculate the Average and Assign a Letter Grade
- Make a function that calculates the average score of the student.
- An if-else statement that determines the letter grade based on the average.
- Display the result in a formatted way.

**Step 4:** Display the Results
- The program prints the name, average score, and assigned grade for each student.

```bash
OUTPUT MAY LOOK SIMILAR TO THIS:
Student Grade Calculator
Enter number of students:
2
Enter student name:
Alice Go
Enter three scores (separate by space):
85 90 80
Alice Go: Average = 85, Grade = B

Enter student name:
Bob Builder
Enter three scores (separate by space):
70 75 72
Bob Builder: Average = 72, Grade = C
Grade calculation completed!
```
