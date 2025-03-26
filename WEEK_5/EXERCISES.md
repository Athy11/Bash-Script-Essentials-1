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
### SED
**EXERCISE 1: Replace "Charlie" with "Charles"**
```bash
sed 's/Charlie/Charles/' students.csv

OUTPUT:
Ana,20,A
Bob,21,B
Charles,22,A
David,19,C
Eve,20,B
```
**EXERCISE 2: Delete students with grade "C"**
```bash
sed '/,C$/d' students.csv

OUTPUT:
Ana,20,A
Bob,21,B
Charlie,22,A
Eve,20,B
```
### AWK
**EXERCISE 1: Extract only names from the file**
```bash
awk -F ',' '{print $1}' students.csv

OUTPUT:
Ana
Bob
Charlie
David
Eve
```

**EXERCISE 2: Display students older than 20**
```bash
awk -F ',' '$2 > 20' students.csv

OUTPUT:
Bob,21,B
Charlie,22,A
```

**EXERCISE 3: Show names and grades only**
```bash
awk -F ',' '{print $1, $3}' students.csv

OUTPUT:
Ana A
Bob B
Charlie A
David C
Eve B
```
