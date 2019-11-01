# Operators and Loops

Operators and loops are essential programming paradigms in controlling the logic of your script or program.  In conjunction with operator's conditions, loops can perform a wide range of powerful computations.  As programmers we can automate tasks to within loops to achieve desired results.  

### Operators

Comparison operators perform evaluations on value(s) to determine an outcome.  Often you will want your program to behave based upon a value's relation to another value.  Here are some of the basic operators that you will utilize in your programs.

>    greater than
<    less than
>=   greater than or equal to
<=   less than or equal to
==   equal to
===  strict equal to
!=   not equal to

### Loops

Loops allow a program to continue performing a function as long as the loop condition has been met.  This is especially powerful when you need the same set of instructions to repeat until a desired result has been achieved.  The two most fundamental loops are known as the ```for``` and ```while``` loops.

#### For loop

The ```for``` loop is a conditional statement that will repeat as long as the statement in the for loop is true.
```
for (var count=0; count < 6; count++>) {
    document.write("Number: " + count);
    document.write("</ br>");
}
```
In this example we are declaring a variable ```count``` and initializing it with the value of 0.  I specified that I want the loop to continue as long as ```count``` is less than ```<``` the value of 10.  Then I stated that for every loop, I want the variable ```count``` to increase by one.

Inside the body of the loop I have a pair of statements that utilizes the variable ```count```.  For every loop, the ```count``` variable will increase by the value of 1.  The second statement will ensure that each loop will be displayed on its own line.  The result of this statement would look similar to this.
```
Number: 1
Number: 2
Number: 3
Number: 4
Number: 5
```
At this stage in the program the ```count``` variable stores the value of ```6```.  Since we declared the loop to terminate when ```count``` is less than 6, the sequence is finished and the program will continue on if more statements exist after the foor loop.

#### While loop

The while loop has similar behavior as a for loop.  As stated in the name, the loop will continue as long as the *while* condition hasn't been met.
```
var count = 50;
while (count <= 0) {
    document.write("Count now is: " + count);
    document.write("</ br>");
    count = count - 10;
}
```
In this example the while loop will continue as long as ```count``` is greater than or equals to ```<=``` 0.  If this condition evaluates to true, then the body of the while loop is executed.  We can expect this output.
```
Count now is: 50
Count now is: 40
Count now is: 30
Count now is: 20
Count now is: 10
Count now is: 0
```
Within the last iteration of this loop, the ```count``` value is ```-10```.  At this stage the *continuation* condition is now false and the while loop is terminated.

[Back to Home Page](index.md)