# TRSGPR-CPU 2022
**Very important note: This specific version will no longer be maintained and will be a read-only archive repository, effective by January 31, 2023. A whole new rewrite is planned from the ground up to clean up a lot of things and learn from the mistakes that were made here.**

The Relatively Simple General-Purpose Register CPU (or TRSGPR-CPU for short) is an amateur university project with the goal of emulating a very simplified version of the GPR-CPU architecture, demonstrating the capabilities of handling two operand instructions. For simplicity's sake, there are features of the GPR-CPU that are not included or supported to simply demonstrate the focal point of this simulation, in which to demonstrate two operand instructions, in contrast to the presented RSCPU (single operand) and the stack-based architectures.

## Changelog - What's New? (0.2.1-alpha build 11w3a)
- ( - ) Removed implementation of ShellExecute() and its subsequent parent library for security reasons.

## How to Run Simulator
This repository unfortunately does not have a packaged executable file within it, however, attempting to run the project is relatively simple. Simply open up the `main.cpp` file within this repository in an IDE you prefer to write your C++ code in and simply build the program yourself. Once you get to successfully build the program, you should expect to be greeted with the console main menu:
![image](https://user-images.githubusercontent.com/82251402/198719396-069ae6e4-399e-4ec4-ab95-6cef2c4867a2.png)

Congratulations! You can now start getting to work with the simulator itself.

## Available Instructions
Due to the nature of the simplification of our project and a deliberate decision by the contributors, we've decided on implementing a grand total of 5 essential instructions for demonstration purposes:
![image](https://user-images.githubusercontent.com/82251402/198722750-60c9b72a-6203-4cdd-90ac-da5daa6739cd.png)
- `ADD  OP1, OP2` - Adds the value from OP2 to OP1, OP1 must not be an immediate value.
- `SUB OP1, OP2` - Subtracts the value from OP2 to OP1, OP1 must not be an immediate value.
- `MOV OP1, OP2` - Moves the value from OP2 to OP1, OP1 must not be an immediate value.
- `INC OP1` - Increments OP1, OP1 must not be an immediate value.
- `JUMP LABEL` - Jumps to a label defined elsewhere other than `start:`
- `DEC OP1` - Decrements OP1, OP1 must not be an immediate value.
- `HLT` - Terminates the process or the program itself.

Once you feel like you're finished, end the input stream by entering `-endstream`.

## Extra Notes
This development stage of our project is notoriously unstable when the user decides to go off the intended use of the program, this will be fixed soon in later editions.
This project will still be maintained and updated regularly as see fit so if you are interested on how this will go, you can star this repository and check from time to time.
