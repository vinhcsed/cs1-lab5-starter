# CS1: Lab 4

## Setup
1. Update the contents of *ID.txt* with your identifier (school email **without @school.edu**).
2. Write pseudocode for your program in *PSEUDO.txt*.

## How to Run Your Program
* [**WINDOWS**] In VSCode, press the play button in the top right corner (it should appear when you open a `.cpp` file). Your program should compile and run.
* [**MAC/LINUX**] Open a Terminal. Type `make` and press return. Your program should compile and run.

## Assignment Specification
### Least, Greatest, and Average
* Implement this program in `main.cpp`.
* Write a program that *continuously* lets the user enter a series of positive integers.
* The user should enter `-9999` to signal the end of the series.
* Output the number of integers entered, the least and greatest integers entered, and the average of all integers entered in the series.
   - The average should be formatted to two decimal places.
   - If the user immediately ends the series, an error message should be printed.

#### Example 1
```
Enter an integer: 1
Enter an integer: 5
Enter an integer: 7
Enter an integer: -9999
Numbers Entered: 3
Least: 1
Greatest: 7
Average: 4.33
```

#### Example 2
```
Enter an integer: 1
Enter an integer: -9999
Numbers Entered: 1
Least: 1
Greatest: 1
Average: 1.00
```

#### Example 3
```
Enter an integer: -9999
ERROR: No numbers entered
```

## Submission
1. Remember to *commit* and *push* your changes to this repository.
