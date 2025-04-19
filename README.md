# Java Multi-threading Demo

## Overview

This Java project demonstrates basic multi-threading using the `Runnable` interface. It creates and starts two threads that print incrementing numbers at different intervals.

## File Structure

- **`MyThread.java`**  
  Contains the `MyThread` class that implements the `Runnable` interface. Each thread prints a number starting from a given initial value, incrementing it at a specified interval after a delay.

- **`Main.java`**  
  Contains the `main` method which starts two threads using instances of `MyThread`. 

## How It Works

- The `MyThread` class constructor takes three parameters:
  - `init` – Initial value to start counting from.
  - `increment` – Value by which to increment each time.
  - `delay` – Delay in milliseconds between each print.

- In `Main.java`, two threads are created:
  - The first thread starts from `1`, increments by `2`, and waits for `300ms` between outputs.
  - The second thread starts from `100`, increments by `20`, and waits for `1000ms` between outputs.

- Both threads run in parallel and continuously print values.

## Sample Output

```
1 
100 
3 
5 
7 
120 
9 
...
```

(Note: Actual output may vary depending on thread scheduling.)

## How to Compile and Run

1. Open a terminal and navigate to the directory containing the files.
2. Compile both files:
   ```bash
   javac MyThread.java Main.java
   ```
3. Run the program:
   ```bash
   java Main
   ```

## Notes

- The threads run infinitely unless manually terminated.
- This project is intended for learning purposes and demonstrates concurrency basics in Java.
