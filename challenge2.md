# PHP Syntax Guide

## PHP Comments:

Used to describe an element in the document without effecting the document. These are used in other programming languages as well.

**ex.**

// Option 1 for single-line comment
\# Option 2 for single-line comment
/*
This is a...
multi-line comment
*/


## PHP Variables:

Used as a container to store information. Variables always start with a '$' symbol. Variables will hold a value which is always followed by a ';' to end the line.

**ex.**

<?php
$txt = "Hello";
?>
*The variable is '$txt'.*


## PHP Echo / Print:

These are used to output data to the screen. 
The difference is...

**Echo:** Has no return value. Can take multiple arguments. Faster.

**ex.**

<?php
echo "<h1>Option 1<h1>"; 
echo "This ", "has ", "multiple arguments/parameters.";
?>

*OR with a key.*

<?php
$txt = "Option 2";
$x = 2
$y = 2

echo "<h1>" . $txt . "</h1>";
echo $x + $y;
?> 

**Print:** Return value is 1. Can take one argument. Slower.

**ex.**

*The echo examples work the same with print except the multiple arguments/parameters example.


## PHP Data Types

Variables can store different types of data. These include:

**String:** Can be any text inside quotes.
**ex.** "Hello World!"

**Integer:** A number without a decimal point. Can be positive or negative.
**ex.** $x =100
var_dump($x);

**Float:** A number with a decimal point.
**ex.** $x =100.11
var_dump($x);

**Boolean:** True or False.
**ex.** $x = true;
$y = false;

**Array:** Multiple values in a single variable.
**ex.** $fruit = array("blueberries","avocado","mango","pineapple");
var_dump($fruit);

**Object:** An item that shares the same classes but has different properties.
**ex.**
 <?php
    class Pet {
    public $color;
    public $animal;
    public function __construct($color, $animal) {
        $this->color = $color;
        $this->animal = $animal;
    }
    public function message() {
        return "My pet is a " . $this->color . " " . $this->animal . "!";
    }
    }

    $myPet = new Pet("black", "cat");
    echo $myPet -> message();
    echo "<br>";
    $myPet = new Pet("white", "dog");
    echo $myPet -> message();
?> 

**NULL:** A variable with no value assigned to it.
**ex.** $x = null;


## PHP Constants:

These are like variables. The difference is that they cannot be changed or undefined.


## PHP Operators:

Are used to perform operations on variables and values. 

The different groups of operators include:

**Arithmetic:** Addition(+), Subtraction(-), Multiplication(*), Division(/), Modulus(%), Exponentiation(**)

**Assignment:** =, +=, -=, *=, /=, %=

**Comparison:** Equal(==), Identical(===), Not Equal(!=)or(<>), Not identical(!==), Greater than(>), Less than(<), Greater than or equal to(>=), Less than or equal to(<=), Spaceship(<=>)

**Increment/Decrement:** Pre-increment(++$x), Post-increment($x++), Pre-decrement(--$x), Post-decrement($x--)

**Logical:** And(and, &&), Or(or, ||), Xor(xor), Not(!)

**String:** Concatenation(.), Concatenation assignment(.=)

**Array:** Union(+), Equality(==), Identity(===), Inequality(!=, <>), Non-identity(!==)

**Conditional Assignment:** Ternary(?:), Null Coalescing(??)


## PHP If & Else & Elseif:

**if:** If the first condition is true this code runs.
**elseif:** If the first condition was false but the second condition is true this code runs.
**else:** If all conditions are false this code runs.


## PHP Functions:

Has over 1000 built-in functions and you can also create your own. Functions are statements you can use repeatdely in a program. You have to call the function to have it load.


## PHP Loop:

Loops are used for a function that you want to repeat multiple times. Instead of rewriting the code over and over again you can add a loop. The loop types include *while, do...while, for, foreach.*