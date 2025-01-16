# Uncommon COBOL Logic Error: Infinite Loop

This repository demonstrates a subtle logic error in a COBOL program that leads to an infinite loop.  The error is not immediately obvious and highlights the importance of careful conditional statement design in COBOL programs.

## Bug Description

The COBOL program contains a `GO TO` statement that jumps back to the `PROCEDURE-DIVISION` without a proper condition to stop the loop. This creates an infinite loop, resulting in the program never terminating.  This type of error is particularly difficult to detect without close examination of the control flow.

## Solution

The solution involves the correct implementation of a conditional statement that ensures the program's termination under the defined condition. A `PERFORM` statement could also be used as a structured programming alternative.