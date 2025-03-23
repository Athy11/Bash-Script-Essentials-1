# FUNCTIONS AND MODULAR PROGRAMMING
Functions in Bash allow you to write reusable blocks of code that can be called multiple times within a script, improving organization and reducing redundancy. Modular programming takes this further by splitting code into separate files (modules) that can be sourced when needed, making scripts more maintainable and scalable.

## Functions in Bash
A function in Bash is a named block of code that performs a specific task and can be executed whenever needed. Using functions helps break down complex scripts into smaller, manageable parts, making the script easier to read and debug. In creating a function, you can do it with or without the keyword **function**.

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
