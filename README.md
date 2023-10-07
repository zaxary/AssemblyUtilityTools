# AssemblyUtilityTools

Welcome to the AssemblyUtilityTools repository! This repository contains two distinct, yet fascinating projects written in assembly language. These projects demonstrate the power and flexibility of assembly language programming, and they serve as excellent learning resources for those interested in low-level programming.

## Project 1: ASCII Art Printer

The first project in this repository is an ASCII Art Printer. This program is designed to print ASCII characters in a large 8-character by 16-character font. It takes characters specified at memory locations x5000 for the 'zero'-bit or negative characters and x5001 for the 'one'-bit or positive characters. It then draws an ASCII character specified at memory location x5002 using the FONT_DATA at the end of the program.

The program uses several registers for different purposes, including holding ASCII values, serving as counters for the column and row, holding the address of FONT_DATA, holding font data for each line, and holding the ASCII value of the character that we need to print. The program starts by initializing these registers and then enters a loop where it loads the value of the character that needs to be printed, sets up encoding for the row and column, and prints the character.

## Project 2: Factorial Calculator

The second project in this repository is a Factorial Calculator. This program calculates the factorial of a number, which is the product of all positive integers less than or equal to that number. The program uses a nested loop structure to perform the multiplication operation through repeated addition. The outer loop decrements the input number until it reaches 1, and the inner loop performs the multiplication of the current number by adding it to itself the appropriate number of times.

The program starts at memory location x3000, loads the input number into a register, initializes a counter for the outer loop, and then enters the outer loop. Inside the outer loop, it enters the inner loop where it increments the sum by the input number and decrements the inner count. Once the inner loop finishes, it updates the sum result from the inner loop, clears the sum to 0, and decrements the outer count. Once the outer loop finishes, it stores the result into a memory location.

## Getting Started

To get started with these projects, clone this repository to your local machine. You will need an assembly language compiler to compile and run these programs. If you want to calculate the factorial of a different number in the Factorial Calculator, you can change the value at the memory location labeled INPUT in the program.
