## DATA PROCESSING AND TEXT MANIPULATION EXAMPLE

This file contains all the student's information and will be used for all of the examples of *grep* *sed* *awk*. It is separated by newline character *\n* with -e as it enables the interpretation of escape sequences, like \n, \t.
```bash
echo -e "Ana,20,A\nBob,21,B\nCharlie,22,A\nDavid,19,C\nEve,20,B" > students.csv
```

### GREP
**EXERCISE 1: Find all students with grade "A"**
```bash
grep ",A$" students.csv

OUTPUT:
Ana,20,A
Charlie,22,A 
```

**EXERCISE 2: Count how many students have grade "B"**
```bash
grep -c ",B$" students.csv

OUTPUT:
2
```

**EXERCISE 3: Find students whose names start with "C"**
```bash
grep "^C" students.csv

OUTPUT:
Charlie,22,A
```
