# BasicJavaTest

# BasicJavaRecap

This recap exercise was produced by Professor Kitlei Robert


Warm-up exercises
-----------------

1. Make a "Hello world" program.

2. Working with command line arguments...
    1. print how many of them there are.
    2. print them in order line by line
    3. print them in order line by line, with sequence numbers
    4. print them in reverse order
    5. print their lengths
    6. supposing that they are all numbers...
        * print their sum
        * print only the even numbers
        * print them in numerical order
    7. print them in alphabetical order
    8. print only those of which there are multiple copies

3. After that...
   1. Make a Fibonacci function, using the recursive definition.
   2. Make another version that uses iteration.
   3. Make another version that returns all the numbers up to the given value in an array.

4. Print all divisors of the number given in the first command line argument.

5. a. Find the function that takes the square root of numbers.
   b. If you have learned about Newton's method, make your own version using it.

6. The command line arguments contains an expression in reverse Polish notation,
   which consists of the four basic operations and integers.
   Calculate the value of the expression.

   Example:         1 2 3 * +

   Result:          7           = (3 * 2) + 1
   

Using OO
-----------------

1. Pairs of command line arguments describe coordinates of points. Print the coordinates of the point that is farthest away from (0,0).

2.  Points are given as before.
    Print the closest point to the first one (excluding itself).

3. Print the command line arguments
    so that consecutive 'a' characters are replaced by a single 'a' in them.
    Look at the documentation of String for an appropriate function.

4. The first command line argument is a text, all other arguments contain two characters.
    Change all occurrences of the first characters to the second ones in the text.

5. Print the first n lines of Pascal's function,
    where n is a command line argument.

6. Let us make a board of size n times m.
    Shots are fired at the board, their coordinates are given similar to Exercise 1a.
    Draw the table so the 'X' marks fields that are hit and '.' otherwise.
6. Let us simulate a direct elimination tournament.
    Our command line arguments are grouped the following way.

    - The first argument is the number of players (n).
      This number is always a power of two: 1, 2, 4, 8, 16...
    - The next n arguments are the names of the players.
    - The remaning n-1 arguments indicate the results of the matches.

      The first round has n/2 matches, the second one n/4, n/8, n/16 and so on,
      until the last round (the final).

      A '1' in the argument means that the top player wins the match,
      and a '2' means that the bottom one wins the match.

    The program has to print the results of the tournament in the following way.

    Example: if the input is        8 J1 J2 J3 J4 J5 J6 J7 J8 1 1 1 2 1 2 2
     then the output is

          J1 J1 J1 J8
          J2
          J3 J3
          J4
          J5 J5 J8
          J6
          J7 J8
          J8

          round 1, players: J1 and J2, advances: J1, eliminated: J2
          round 1, players: J3 and J4, advances: J3, eliminated: J4
          round 1, players: J5 and J6, advances: J5, eliminated: J6
          round 1, players: J7 and J8, advances: J8, eliminated: J7
          round 2, players: J1 and J3, advances: J1, eliminated: J3
          round 2, players: J5 and J8, advances: J8, eliminated: J5
          round 3 (final), players: J1 and J8, champion: J8, finalist: J1
