# Assignment 17

Some perfect squares have unique mathematical properties. For example, 36 is:

1. A perfect square 
2. The sum of the integers 1 to 8 (1+2+3+4+5+6+7+8 = 36)

A number having both of these properties, being a perfect square and equal to the sum of consecutive integers beginning with 1, is sometimes referred to as a "magic square."

1 and 36 are the first two magic squares and the next one after 36 is 1225:

1. 35\*35 = 1225
2. 1225 = sum of 1 to 49

## Specifications

* Only one class is needed (with a `main` method and the method `printMagicSquares`, no constructor needed), where the `printMagicSquares` method prints the first n magic squares (see the specifications for the method below).

```
    /** 
     * Prints the first n magic squares (with squared number and integer sum indicated).
     * Ex: 36 (1 to 8)
     *
     * Precondition: n > 0
     * @param n - the number of magic squares to print
     */
    public static void printMagicSquares(int n)
```

* You should only be checking positive integers, so have your program reject invalid inputs in `main`.

* Let the users keep using the program as many times as they would like. Control this in `main`.

### Hints

* You will probably need to use both two `while` loops in your `printMagicSquares` method.

* I have seen two ways of finding the magic squares. One method is slow and one is fast (for n = 6, slow method takes about 6.5 min and fast method takes 0.5 s).

* I would recommend using `long` instead of `int` if you want to test big numbers (max value of `int` is 2,147,483,647 and max value of `long` is 9,223,372,036,854,775,807).

* Pseudo code of possible solution (replace the comments with the appropriate code):

```
public static void printMagics(int n)
{
    int curSqrt = 1;
    int curSum = 0;
    int curAdd = 0;
        
    // while loop until n magic squares have been found
            
        int square = // generate perfect square
            
        // while loop to keep going until the next magic square is found
            // increment addend [used in sum]
            // add that next int to sum
                
            // check if it is impossible for sum to be equal to square
                // curSqrt++;
                // update square
        
        // print magic square (and info about the sum)
}
```

### Sample Output

```
Print the first n magic squares: 4
1 (1 to 1)
36 (1 to 8)
1225 (1 to 49)
41616 (1 to 288)
```

```
Print the first n magic squares: 13
1 (1 to 1)
36 (1 to 8)
1225 (1 to 49)
41616 (1 to 288)
1413721 (1 to 1681)
48024900 (1 to 9800)
1631432881 (1 to 57121)
55420693056 (1 to 332928)
1882672131025 (1 to 1940449)
63955431761796 (1 to 11309768)
2172602007770041 (1 to 65918161)
73804512832419600 (1 to 384199200)
2507180834294496361 (1 to 2239277041)
```

### Grading

As always, your program will be graded on its functionality according to the project specifications and proper code style.

