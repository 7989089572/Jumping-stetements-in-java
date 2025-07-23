# Java Jumping Statements Practice

This repository contains a demonstration and explanation of Jumping Statements in Java.

## Theory

### Break Statement
Used to exit a loop or switch statement immediately, stopping further iterations.

### Continue Statement
Skips the current iteration and continues with the next iteration in the loop.

### Return Statement
Exits from a method and optionally returns a value.

---

## Coding Example

See [`JumpingStatements.java`](JumpingStatements.java) for the full code.

```java
public class JumpingStatements {
    public static void main(String[] args) {
        System.out.println("=== Break Statement Example ===");
        for (int i = 1; i <= 10; i++) {
            if (i == 5) {
                System.out.println("Breaking the loop at i = " + i);
                break; // Exits the loop when i equals 5
            }
            System.out.println("i = " + i);
        }

        System.out.println("\n=== Continue Statement Example ===");
        for (int i = 1; i <= 10; i++) {
            if (i == 5) {
                System.out.println("Skipping the value i = " + i);
                continue; // Skips the rest of the loop when i equals 5
            }
            System.out.println("i = " + i);
        }

        System.out.println("\n=== Return Statement Example ===");
        JumpingStatements obj = new JumpingStatements();
        obj.printNumbers();
    }

    public void printNumbers() {
        for (int i = 1; i <= 10; i++) {
            if (i == 7) {
                System.out.println("Returning from method at i = " + i);
                return; // Exits the method when i equals 7
            }
            System.out.println("i = " + i);
        }
    }
}
```

---

## Sample Output

```
=== Break Statement Example ===
i = 1
i = 2
i = 3
i = 4
Breaking the loop at i = 5

=== Continue Statement Example ===
i = 1
i = 2
i = 3
i = 4
Skipping the value i = 5
i = 6
i = 7
i = 8
i = 9
i = 10

=== Return Statement Example ===
i = 1
i = 2
i = 3
i = 4
i = 5
i = 6
Returning from method at i = 7
```
