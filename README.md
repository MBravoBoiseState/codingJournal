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
<sub>Using Classes and Objects</sub>

This chapter we learned about the difference between classes and objects. 

The class construct defines a new type that can group data and methods to form an object. A class' public member methods indicate all operations a class user can perform on the object. *In 3rd grader terminology: a class is a "house blueprint" for different methods to live in and make up different objects*. Keep in mind that a programmer can create one or more objects of the same class.... Please referenece the example code below where 2 different objects are created utilizing the RestaurantFavorites class:

```
public class RestaurantFavorites {
   public static void main(String[] args) {
      Restaurant favLunchPlace = new Restaurant();
      Restaurant favDinnerPlace = new Restaurant();

      favLunchPlace.setName("Central Deli");
      favLunchPlace.setRating(4);

      favDinnerPlace.setName("Friends Cafe");
      favDinnerPlace.setRating(5);

      System.out.println("My favorite restaurants: ");
      favLunchPlace.print();
      favDinnerPlace.print();
   }
}
```

We also took a deep dive into utilizing packages. Ex: ```import java.util.Scanner``` imports the Scanner method from the java.util package.

Utilizing the "*" at the end of an import will import the entire package. Ex: ```import java.util.*``` will import all methods in the java.util package. (AKA known as a wildcard character import)

The last topic we went over in module 3 was output formatting utilizing the printf() method. We learned that we could utilize format specifiers to output information in a specific format. Please review the chart snippets below for review.

![a chart of printf format specifiers](https://github.com/MBravoBoiseState/codingJournal/blob/main/printfFormatSpecifiers.png)

![a chart of printf sub specifiers](https://github.com/MBravoBoiseState/codingJournal/blob/main/printfSubSpecifiers.png)
--------------------------------------------------------------------------------------------------------------------------------------------------------

## Chapter 4 :trollface:
<sub>Conditionals and Loops and other Stuff</sub>

*I am behind on getting these journal notes setup and i know as we get into the semester more they only become more important so i am FORCING myself to catch up....*

Chapter 4 was a bit of a struggle for me honestly (wait for my chapter 5 entry) probably mostly because i was on vacation. There was also A LOT of content on conditionals and loops... i mean a lot. like 30 sections on it. 

The main points I want to take away from this chapter is example code for a switch statement because i know at one point it will be asked and I just don't have this sitting at the top of my head...

```
switch (a) {
  case 0:
     // Print "zero"
     break;

  case 1:
     // Print "one"
     break;

  case 2:
     // Print "two"
     break;

   default:
     // Print "unknown"
     break;
}
```

Next is the different type of loops that are available at my disposal because i thought i knew them all but then i did the following lab and i do not all the loop types there are. The two that I am really comfortable with are while loops and for loops. 

```
for (initialExpression (generally i = 0); conditionExpression (generally something like i <= variable); updateExpression (generally i++ or i--) ) {
  // Loop body
}
// Statements after the loop
```

```
while (expression) { // Loop expression
    // Loop body: Executes if expression evaluated to true 
    // After body, execution jumps back to the "while"
}
// Statements that execute after the expression evaluates to false
```
I could not find anything ZyBooks about Do-While loops BUT Luke did use them in one of the lab walkthroughs so I do want to make note of them here: 

```
int count = 1;
        do {
            System.out.println("Count is: " + count);
            count++;
        } while (count < 11);
```

Straight from the Java Docs. "The difference between do-while and while is that do-while evaluates its expression at the bottom of the loop instead of the top. Therefore, the statements within the do block are always executed at least once" So if I need a While Loop to at least iterate once, then i need to use a Do-While Loop.

Other stuff I wanted to touch base on for this chapter is Variable Name Scope... 

A declared name is only valid within a region of code known as the name's scope. Ex: A variable userNum declared in main() is only valid within main(), from the declaration to main()'s end.

Most of this material declares variables at the top of main() (and if the reader has studied methods, at the top of other methods). However, a variable may be declared within other blocks too. A block is a brace-enclosed {...} sequence of statements, such as found with an if-else, for loop, or while loop. A variable name's scope extends from the declaration to the closing brace }.

TO DUMB IT DOWN A BIT... If a variable exists within a code block, then the variable is only "accesible" within the codeblock unless we are returning the value. Furthermore, it is possible to create duplicate variables but it is not good practice and I will def avoid at all costs. 

<strong>Common Error:</strong>  A variable declared within a loop block is (unexpectedly) re-initialized every iteration.

```
public class ScopeError {
   public static void main (String[] args) {
      int i = 0;

      while (i < 5) {
         int tmpSum = 0;
         tmpSum = tmpSum + i; // Logic error: Sum is always just i
         System.out.println("tmpSum: " + tmpSum);
         i = i + 1;
      }
   }
}
```
--------------------------------------------------------------------------------------------------------------------------------------------------------

## Chapter 5 :face_with_spiral_eyes:
<sub>User-defined Methods, ArrayLists, File Parsing, and Exceptions</sub>

Ok. This chapter is the first instance where I am starting to encounter unfamiliar programming concepts, especially because they are in Java. That's ok though because so far the only thing I am struggling to somewhat understand is EXCEPTION HANDLING. I hope everyone is as confused as i am xD

To start off we learned about methods. we learned to create them. import them. use them. love them. 

Look at the SIMPLE example below: 

```
public class SquareComputation {

   public static int computeSquare(int numToSquare) {
      return numToSquare * numToSquare;
   }

   public static void main (String [] args) {
      int numSquared;

      numSquared = computeSquare(7);
      System.out.println("7 squared is " + numSquared);
  }
}
```
I want to call out for this specific example that the computeSquare method is setup as "public static int" because it is expected to return an int datatype value. The main method is setup as public static void because it is not expected to return any values. If a method (besides the main method) is created that is not expected to return a value but simply just print information to the console then it will be setup as public static void methodExampleName(){};

Something else I'd like to call out about the example is the expected parameter passed through the computeSquare method is ```int numToSquare```. This means that the method expects an int datatype parameter passed through the method when called. This happens in the main method when you see ```numSquared = computeSquare(7);``` 7 is the int datatype parameter passed through the method which is then utilized to fill in whenever numToSquare is used in the computeSquare method. 

UNIT TESTING... Unit testing will be the death of me eventually... 

Unit testing is the process of individually testing a small part or unit of a program, typically a method. A unit test is typically conducted by creating a testbench, a.k.a. test harness, which is a separate program whose sole purpose is to check that a method returns correct output values for a variety of input values. Each unique set of input values is known as a test vector.

The language provides a compact way to print an error message when an expression evaluates to false. Assert is an operator that prints an error message and exits the program if the provided test expression evaluates to false, having the form:

Assert operator is as follows, ```assert testExpression : detailedMessage;```

Please review the sample code to review how to setup unit testing with assertion: 

```
public class HrMinToMinTestHarness {
   public static double hrMinToMin(int origHours, int origMinutes) {
      int totMinutes;      // Resulting minutes

      totMinutes = (origHours * 60) + origMinutes;

      return origMinutes;
   }

   public static void main(String[] args) {
      System.out.println("Testing started");

      assert (hrMinToMin(0, 0) == 0) : "Assertion (hrMinToMin(0, 0) == 0) failed";
      assert (hrMinToMin(0, 1) == 1) : "Assertion (hrMinToMin(0, 1) == 1) failed";
      assert (hrMinToMin(0, 99) == 99) : "Assertion (hrMinToMin(0, 99) == 99) failed";
      assert (hrMinToMin(1, 0) == 60) : "Assertion (hrMinToMin(1, 0) == 60) failed";
      assert (hrMinToMin(5, 0) == 300) : "Assertion (hrMinToMin(5, 0) == 300) failed";
      assert (hrMinToMin(2, 30) == 150) : "Assertion (hrMinToMin(2, 30) == 150) failed";
      // Many more test vectors would be typical...

      System.out.println("Testing completed");
   }
}

```

Note that assertions are not enabled by default. A programmer must execute Java programs with additional command-line options in order to enable assertions. Specifically, the command-line option -ea is necessary at run-time. Ex: java -ea HrMinToMinTestHarness

I will read up more on unit testing once it becomes more prominent within our labs. 

OUTPUT AND INPUT STEAMS ;-;

I am still so very confused about these concepts. I understand the use case and I think I just need some practice with them but also I really want to avoid them at all cost :( 

From what i do understand, input and output stream are great tools for "grabbing" data from user input strings. Here is a super simple example so I don't confuse myself that demonstrates the power of input streams:

```
import java.util.Scanner;

public class StringInputStream {
   public static void main(String[] args) {
      Scanner inSS = null;              // Input string stream
      String userInfo;                  // Input string
      String firstName;                 // First name
      String lastName;                  // Last name
      int userAge;                      // Age

      userInfo = "Amy Smith 19";

      // Init scanner object with string
      inSS = new Scanner(userInfo);

      // Parse name and age values from string
      firstName = inSS.next();
      lastName = inSS.next();
      userAge = inSS.nextInt();

      // Output parsed values
      System.out.println("First name: " + firstName);
      System.out.println("Last name: " + lastName);
      System.out.println("Age: " + userAge);
   }
}

```

ArrayLists was one of the more simple concepts for me to understand this week. I have experience with arrays and array manipulation so this was nice to refresh myself on. I have pasted some code for declaring and adding some data to array lists below: 

```
ArrayList<Integer> valsList = new ArrayList<Integer>();

//Creating space for 3 Integers
valsList.add(31);
valsList.add(41);
valsList.add(59);

System.out.println(valsList.get(1));

// Setting the value of existing elements
valsList.set(1, 119);

System.out.println(valsList.get(1));

```

I do want to call out that ArrayLists must be imported from the java.util package:

```import java.util.ArrayList;```
