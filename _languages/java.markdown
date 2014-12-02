---
layout: language
icon: icon-java

Language: Java
Language_Description: Class based, object oriented programming with few implementation dependencies.


Data_Types:
- Type: int
  Description: Declares an integer.
  Syntax: int variable_name;

- Type: float
  Description:  Declares a variable that's able to harness the power of deciamls (accurate up to 7 digits).
  Syntax: float variable_name;

- Type: double
  Description: Same as float, but is more exact (accurate up to 15 digits).
  Syntax: double variable_name;

- Type: char
  Description: 8 bit data type that usually contains characters.
  Syntax: char variable_name;

- Type: String
  Description: An object that represents sequences of characters.
  Syntax: String variable_name;

Structures:
- Type: if
  Description: Executes code if the following statement is true.
  Syntax: if(statement) {code}
  Example: if(x>5) {code}
  Example_Description: Code will only be executed if the variable x is greater than 5.

- Type: else
  Description: Follows an if block and will be executed if the if block isn't.
  Syntax: else {code}

- Type: else if
  Description: Follows an if block and will be executed if the previous if block wasn't executed and the new parameters are met.
  Syntax: else if (statement) {code}
  Example: else if (x==5) {code}
  Example_Description: Executes when previous if block doesn't and only if x equals 5.

- Type: while
  Description: Repeats code as long as statement remains true.
  Syntax: while (statement) {code}
  Example: while (x>5) {code}
  Example_Description: Code will only execute if x is greater than 5 and will keep looping until x isn't greater than 5.

- Type: do while
  Description: Code executes once and then statement is tested.  If statement remains true the do while will keep looping.
  Syntax: do {code} while (statement)
  Example: do {code} while (x>5)
  Example_Description: Code will execute once and then test if x is greater than 5.  If it is then it'll loop, if not it'll move on.

- Type: for
  Description: Loops as long as the stated conditions are met.
  Syntax: for (variable; condition; increment) {code}
  Example: for (x=0; x<5; x++) {code}
  Example_Description: Evaluates 'x' to equal 0 and loops if x is less than 5.  After each execution the value of x will increase by '+1'.

- Type: switch
  Description: Allows specific code to be used. Variable used must be an integer and the 'vars' must be constant. The switch will jump to the first case that's equal to your stated variable and do the rest of the codes from there (so it'll skip everything before the first case used). Adding a 'break' statement will exit the switch statement if case is satisfied and prevent additional statements from executing. If none of the cases are equal to your variable then it'll only execute the last section of code (the code following 'default').
  Syntax: |
          switch (variable) {
            case var1:
              code;
              break; //exits switch statement, prevents other cases from executing
            case var2:
              code;
            default:
              code;
          }
  Example: |
          int x = 5;
          int var1 = 4;
          int var2 = 5;
          switch (x) {
            case var1:
              code;
              break;
            case var2:
              code:
            default:
              code;
          }
  Example_Description: This switch would skip the first line of code and execute everything after that.

User_Interface:
- Type: System.out.println
  Description: Displays to stdout.
  Syntax: System.out.println(output);
  Example: System.out.println("the value of 'x' is" + x);
  Example_Description: Displays "The value of x is x_value"

Comments:
- Type: Single Line
  Syntax: //comments

- Type: Block
  Syntax: "/*many comments*/"


Hello_World:
- Type: Example
  Example: |-
            public class HelloWorld {
              public static void main(String[] args) {
                System.out.println("Hello, World");
              }
            }
---
