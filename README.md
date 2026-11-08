# Java `while` Loop Example

A minimal Java program that demonstrates a `while` loop, and what happens when the loop variable is never updated.

## What It Demonstrates

```java
int i = 2;
while (i < 5) {
    System.out.println("value of i = " + i);
}
```

A `while` loop checks its condition before each pass and keeps running as long as the condition is true.

## Important: This Program Never Ends

Nothing inside the loop changes `i`, so `i < 5` stays true forever. The program prints the same line again and again until you stop it:

```
value of i = 2
value of i = 2
value of i = 2
...
```

This is called an **infinite loop**. To stop the program, press `Ctrl + C` in the terminal, or use the stop button in your IDE.

## The Fix

Add `i++` inside the loop so the variable moves toward the point where the condition becomes false:

```java
int i = 2;
while (i < 5) {
    System.out.println("value of i = " + i);
    i++;
}
```

Output:

```
value of i = 2
value of i = 3
value of i = 4
```

When `i` reaches `5`, the condition `i < 5` is false and the loop ends.

## Requirements

- Java Development Kit (JDK) 8 or higher

## Getting Started

### Clone the repository

```bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
```

### Compile

```bash
javac While_Loop.java
```

### Run

```bash
java While_Loop
```

## Tips for Writing `while` Loops

- Make sure something inside the loop changes the condition
- Check the starting value of the variable
- Use `break` to exit a loop early if needed

## Project Structure

```
.
├── While_Loop.java
└── README.md
```

## Next Steps

- Count down with `i--`
- Use a `while` loop to add up the numbers from 1 to 100
- Compare with `do-while` and `for` loops
