# Coding Journal :computer:  
<sub> The Homies Begged </sub>

---------------------------------------------------------------------------------------------------------------------------------------------------------

## Chapter 1   :blue_book:
<sub>Brief Intro to Programming </sub>

#### Definitions
Input: A program gets data, perhaps from a file, keyboard, touchscreen, network, etc.  
Process: A program performs computations on that data, such as adding two values like x + y.  
Output: A program puts that data somewhere, such as to a file, screen, network, etc.  
Computational thinking: creating a sequence of instructions to solve a problem. 
Algorithm: sequence of instructions that solves a problem. 
Syntax error: is to violate a programming language's rules on how symbols can be combined to create a program. A syntax error is known as a type of compile-time error.  
Logic error: also called a bug, is an error that occurs while a program runs. 


#### Concepts
When thinking about how programs will execute you'll want to think like you're analyzing a cooking recipe. Step by step. Increment by increment.   
The following code at the top of a file enables the program to get input: import java.util.Scanner;  
DON'T FORGET YOUR SEMICOLONS!!!   
A single-line comment starts with // and includes all the following text on that line. Single-line comments commonly appear after a statement on the same line.  
A multi-line comment starts with /* and ends with */, where all text between /* and */ is part of the comment. A multi-line comment is also known as a block comment.  
Work errors in order that you receive them (work top lines first). If you are not seeing an error in the referenced line, look at earlier lines within your code.  

---------------------------------------------------------------------------------------------------------------------------------------------------------

## Chapter 2   :triangular_ruler:
<sub>Data & Expressions ;-; </sub>

*I am still trying to figure out how I want to structure this as I feel like the structure I used for chapter 1 will not work well with the type of learner I am so please bare with me (yourself) if the Chapter note style varies.... Also. Please don't forget your semicolons*

This chapter we learned about data types. I am currently struggling with the character (Char) datatype, gathering input from a user (will watch youtube video for Java breakdown), and other methods readily available in Java. 

Below is an example block for gathering user input and boilerplate for future reference: 


```
import java.util.Scanner;

public class Salary {
   public static void main(String [] args) {
      int wage;

      Scanner scnr = new Scanner(System.in);
      wage = scnr.nextInt();

      System.out.print("Salary is ");
      System.out.println(wage * 40 * 52);
   }
}
```
The lab for this chapter was great practice for getting user input because after the lab I had a better understanding of how it works. 

![A gif to express my mind blowing epiphany](https://github.com/MBravoBoiseState/codingJournal/blob/main/mindBlown.gif)

It seems that the ```Scanner scnr = new Scanner(System.in);``` line is to assign the method to a variable for future use throughout the program.
I became way more comfortable combining the scnr method with a print statement to get user input. 

Another thing that was nice to get practice with was some datatype conversion. In this lab I converted int datatypes into double datatypes so the final print statement would print out a result that was not rounded. Please see the line below for an example of the data conversion: 

```decimalConversion = (double)numerator / (double)denominator;```

#### Guided Experimentaion Notes

- The way your expressions are built, in the sense of order of operations, really matters and can greatly impact the results you are receiving. Reference Example code below: 

```
public class ConversionFun {
    public static void main(String[] args) {
        final double PI = 3.14159;
        double radiusCubed = 1.0;
        double volume1 = 4 / 3 * PI * radiusCubed;
        double volume2 = PI * radiusCubed * 4 / 3;
        double volume3 = PI * radiusCubed * (4 / 3);
        double volume4 = 4 / (3 * PI) * radiusCubed;

        System.out.println("Volume 1: " + volume1);
        System.out.println("Volume 2: " + volume2);
        System.out.println("Volume 3: " + volume3);
        System.out.println("Volume 4: " + volume4);
        
    }
}
```
- Datatypes are important. Need to take into consideration the situation and use the appropriate datatypes when necessary. Reference example below: 

12/5 as integer datatypes = 2 (it's actually 2.4 but the int datatype drops the decimal)

12/5 as double datatypes = 2.4

- Datatypes can also affect how results/variables are printed/returned to the terminal.

- The final operator does not allow to print to the terminal (need to look further into this) 


--------------------------------------------------------------------------------------------------------------------------------------------------------

## Chapter 3   :robot:
