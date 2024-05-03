# Python-a

Python - popular programming language.
    -created by Guido van Rossum: released in 1991.

Used for:
  -web development (server-side),
  -software development,
  -mathematics,
  -system scripting- write programs that automate tasks related to the operating system, like managing files, folders, programs, and system settings.
                   - Python has special tools, called modules, such as os and shutil, that help with these tasks by providing ready-to-use functions.

What can Python do:
    -Python can be used on a server to create web applications.
    -Python can be used alongside software to create workflows.
    -Python can connect to database systems. It can also read and modify files.
    -Python can be used to handle big data and perform complex mathematics.
    -Python can be used for rapid prototyping, or for production-ready software development.


Why Python?
    -Python works on different platforms (Windows, Mac, Linux, Raspberry Pi, etc).
    -Python has a simple syntax similar to the English language.
    -Python has syntax that allows developers to write programs with fewer lines than some other programming languages.
    -Python runs on an interpreter system, meaning that code can be executed as soon as it is written. This means that prototyping can be very quick.

Python Syntax:
    Python Indentation:
        -Python will give you an error if you skip the indentation:
            
            *correct indentification*
            
              -if 5 > 2:
                  print("Five is greater than two!")
                  
            *wrong indetification = error*
                if 5 > 2:
                print("Five is greater than two!")

                -CODE THROWS AN ERROR
                
    *CODE THROWS AN ERROR*
          if 5 > 2:
 print("Five is greater than two!")
        print("Five is greater than two!")
        

        - correct code, both print statements are indented at the same level, which is the correct way to write it in Python.
            -if 5 > 2:
    print("Five is greater than two!")
    print("Five is greater than two!")



Python Variables:
    -variables are created when you assign a value to it. 
    -has no command for declaring a variable.
        -example: 
          -x = 5 # automatically int data type
          -y = "Hello, World!" # string data type

    - keyword to make the variable x belong to the global scope.
        -"GLOBAL"
           To make a variable global in Python, you need to use the GLOBAL keyword inside a FUNCTION 
               -Here's an example:
               
                - def my_function():
                      global x
                      x = 10

                  my_function()
                  print(x)

        *Casting*
            -If you want to specify the data type of a variable, this can be done with casting.
                -example:
                      x = str(3)    # x will be '3'
                      y = int(3)    # y will be 3
                      z = float(3)  # z will be 3.0

            - Specify a Variable Type:
            
                  -int(): Constructs an integer number. It can take an integer literal, a float literal (by removing all decimals), or a string literal (providing the string represents a whole number). 
                          -int(5.8) would result in 5, and int('10') would result in 10.
                  -float(): Constructs a float number. It can take an integer literal, a float literal, or a string literal (providing the string represents a float or an integer).
                          -float(5) would result in 5.0, and float('3.14') would result in 3.14.
                  -str(): Constructs a string from a wide variety of data types, including strings, integer literals, and float literals. 
                          -str(10) would result in '10', and str(3.14) would result in '3.14'.

              EXAMPLES OF CASTING
                  - Integers:

                            x = int(1)   # x will be 1
                            y = int(2.8) # y will be 2
                            z = int("3") # z will be 3

      - QUOTES
            -x = "John"
           IS THE SAME AS
            x = 'John'
            
      - CASE SENSITIVE
          Variable names are case-sensitive.
            - a = 4
              A = "Sally"
              #A will not overwrite a
                - THESE ARE TWO DIFFERENT VARIABLES.

      - Multi Words Variable Names
          -Camel Case
            -myNameTag
              -starts with lowercase letter
          -Pascal Case
            -MyNameTag
              -starts with uppercase letter
          -Snake Case
            -my_name_tag
            
   OUTPUT VARIABLES
           -print() function is often used to output variables
               -x = "Python is awesome"
               print(x)
          -  print() function
                  - when you try to combine a string and a number with the + operator Python will give you an ERROR!
                   EXAMPLE:x = 5
                           y = "John"
                           print(x + y)
Comments in Python:
    - comments start with the # symbol, and anything after the # on that line is treated as a comment and is ignored by the Python interpreter

  *Multiline Comments*
    -there is no specific syntax for multiline comments like in some other programming languages. 
    -you can use a # at the beginning of each line to create a multiline comment. 
        - #This is a comment
          #written in
          #more than just one line
          print("Hello, World!")

          OR
    -You can use multiline string (enclosed in triple quotes) to create multiline comments in Python. 
    -Since Python ignores string literals that are not assigned to a variable or used in an expression.


Python - Modify Strings
    -Remove Whitespace
        - USE strip() METHOD
            -a = " Hello, World! "
                print(a.strip()) # returns "Hello, World!"

    - Replace String
        -Replacing characters in a string.
            - USE replace() METHOD
                -a = "Hello, World!"
                    print(a.replace("H", "J"))
                    =Jello, World!
                    
     - Split String
         -Splits the string into substrings if it finds instances of the separator:
         -USE split() METHOD
             -a = "Hello, World!"
                print(a.split(",")) # returns ['Hello', ' World!']
                 
                     
    -String Concatenation
        -String Concatenation
            - combine, two strings you can use the + operator.
            - a = "Hello"
                b = "World"
                c = a + b
                print(c)
                
                =HelloWorld

        -To add a space between them, add a " ":

                    a = "Hello"
                    b = "World"
                    c = a + " " + b
                    print(c)
​
                    = Hello World
       
        STRING FORMAT:
         -
PYTHON METHODS
    -In programming you often need to know if an expression is True or False.
    -You can evaluate any expression in Python, and get one of two answers, True or False.



    Python Operators
    SAME AS WHAT YOU KNOW!!!
    

Python If ... Else
        
ADD ON TO WHAT YOU KNOW ABOUT IF STATEMENTS: 
    - Elif
        -The elif keyword is Python's way of saying "if the previous conditions were not true, then try this condition".
              a = 33
              b = 33
              if b > a:
                  print("b is greater than a")
              elif a == b:
                  print("a and b are equal")

                  = a and b are equal

                  
  The pass Statement
     -if statements cannot be empty.
     if EMPTY = put in the pass statement to avoid getting an error.

         a = 33
        b = 200
        if b > a:
          pass

Python While Loops
     -Python Loops
        Python has two primitive loop commands
            -while loops
                    -With the while loop we can execute a set of statements as long as a condition is true.
                            -Print i as long as i is less than 6:
                                    i = 1
                                    while i < 6:
                                      print(i)
                                      i += 1

                                    OUTPUT
                                    1
                                    2
                                    3
                                    4
                                    5

    -The break Statement
            - With the break statement we can stop the loop even if the while condition is true. 

            Example
                Exit the loop when i is 3:
                
                i = 1
                while i < 6:
                  print(i)
                  if i == 3:
                    break
                  i += 1
ANSWERS
                1
                2
                3

    -The continue Statement
        -With the continue statement we can stop the current iteration, and continue with the next:

                    -Example
                       - Continue to the next iteration if i is 3:
                    
                        i = 0
                        while i < 6:
                          i += 1
                          if i == 3:
                            continue
                          print(i

                    -OUTPUT
                    1
                    2
                    4
                    5
                    6

        -The code uses a while loop to count from 1 to 6. However, when the count reaches 3, it skips printing that number and continues to the next one. This is            -because of the continue statement, which tells the loop to skip the rest of the code inside the loop for that iteration and move to the next iteration.
               
                
        -for loops
        -
            








    
      
