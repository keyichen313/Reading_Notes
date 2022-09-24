# Reading Notes for 7

## First Article: Control Flow

### Definition for Control flow

>The control flow is the order in which the computer executes statements in a script.

>Control flow means that when you read a script, you must not only read from start to finish but also look at program structure and how it affects order of execution.

## Second Article: JavaScript Functions 

### Definition for function

>A JavaScript function is a block of code designed to perform a particular task.

>A JavaScript function is executed when "something" invokes it (calls it).

1. Function Syntax

>>A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().

>>Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).

>>The parentheses may include parameter names separated by commas:
(parameter1, parameter2, ...)

>>The code to be executed, by the function, is placed inside curly brackets: {}

>> Function parameters are listed inside the parentheses () in the function definition.

>>Function arguments are the values received by the function when it is invoked.

>>Inside the function, the arguments (the parameters) behave as local variables.

2. Function Invocation

The code inside the function will execute when "something" invokes (calls) the function: when user clicks, when called from JS code, when self invoked.

3. Function Return

When JS reaches a return statement, the function will stop executing

4. Why Functions?

You can reuse the code, define the code once, and use it many times.

5. The () Operator Invokes the Function
    
    <pre>
    function FUNCTION_OBJECT(FUNCTION_RESULT){
        return (******);
    }
    document.getElementById("demo").innerHTML = FUNCTION_OBJECT;
    </pre>

6. Functions Used as Variable Values

Functions can be used the same way as you use variables, in all types of formulas, assignments, and calculations

<pre>
<script>
document.getElementById("demo").innerHTML =
"The temperature is " + toCelsius(77) + " Celsius";

function toCelsius(fahrenheit) {
  return (5/9) * (fahrenheit-32);
} 
</script>

result::The temperature is 25 Celsius
</pre>

7. Local VVariables

variables declared within a JavaScript function, become LOCAL to the function(only can be used inside the {})

## Third Article: JavaScript Operators

<pre>
Operator	Description
+	    Addition
-	    Subtraction
*	    Multiplication
**	    Exponentiation (ES2016)
/	    Division
%	    Modulus (Division Remainder)
++	    Increment
--	    Decrement

Operator Ex     Same As
=	    x = y	    x = y
+=	    x += y	    x = x + y
-=	    x -= y	    x = x - y
*=	    x *= y	    x = x * y
/=	    x /= y	    x = x / y
%=	    x %= y	    x = x % y
**=	    x **= y	    x = x ** y
</pre>

>Adding JavaScript Strings
The + operator can also be used to add (concatenate) strings.

>Adding Strings and Numbers
Adding two numbers, will return the sum, but adding a number and a string will return a string

>JavaScript Comparison Operators
<pre>
Operator	Description
==	    equal to
===	    equal value and equal type
!=	    not equal
!==	    not equal value or not equal type
    >   greater than
<	    less than
    >=	greater than or equal to
<=	    less than or equal to
?	    ternary operator

>JavaScript Logical Operators
Operator	Description
&&	        logical and
||	        logical or
!	        logical not
</pre>

>JavaScript Type Operators
Operator	Description
typeof	    Returns the type of a variable
instanceof	Returns true if an object is an instance of an object type


>JavaScript Bitwise Operators
Bit operators work on 32 bits numbers.

>Any numeric operand in the operation is converted into a 32 bit number. The result is converted back to a JavaScript number.
<pre>
Operator	Description	            Example	    Same as	        Result	    Decimal
&	        AND	                    5 & 1	    0101 & 0001	    0001	    1
|	        OR	                    5 | 1	    0101 | 0001 	0101	    5
~	        NOT         	        ~ 5	        ~0101	        1010	    10
^	        XOR	                    5 ^ 1	    0101 ^ 0001	    0100	    4
<<	        left shift	            5 << 1	    0101 << 1	    1010	    10
>>	        right shift	            5 >> 1	    0101 >> 1	    0010	    2
>>>	        unsigned right shift	5 >>> 1	    0101 >>> 1	    0010	    2
</pre>

## Fourth Article: Expressions and Operators

### At a high level, an expression is a valid unit of code that resolves to a value. There are two types of expressions: those that have side effects (such as assigning values) and those that purely evaluate.
<br>


### JavaScript has both binary and unary operators, and one special ternary operator, the conditional operator. A binary operator requires two operands, one before the operator and one after the operator: 
<pre>operand1 operator operand2</pre>

### A unary operator requires a single operand, either before or after the operator:

<pre>operator operand
operand operator</pre>

1. assigning to properties:
   <br>
   If an expression evaluates to an object, then the left-hand side of an assignment expression may make assignments to properties of that expression.

2. Destructuring
<br>
make it possible to extract data from arrays or objects using a syntax that mirros the construction of array and object literals.

3. Evaluation and nesting
<br>
In general, assignments are used within a variable declaration (i.e., with const, let, or var) or as standalone statements).

4. Avoid Assignment Chains
<br>
const z = y = x = f()
> This statement seemingly declares the variables x, y, and z. However, it only actually declares the variable z. y and x are either invalid references to nonexistent variables 

5. Comparison Operators

6. Arithmetic Operators

7. Bitwise Operators

>A bitwise operator treats their operands as a set of 32 bits (zeros and ones), rather than as decimal, hexadecimal, or octal numbers. For example, the decimal number nine has a binary representation of 1001. Bitwise operators perform their operations on such binary representations, but they return standard JavaScript numerical values.

8.Bitwise shift operators
>
The bitwise shift operators take two operands: the first is a quantity to be shifted, and the second specifies the number of bit positions by which the first operand is to be shifted. The direction of the shift operation is controlled by the operator used.

Shift operators convert their operands to thirty-two-bit integers and return a result of either type Number or BigInt: specifically, if the type of the left operand is BigInt, they return BigInt; otherwise, they return Number.

9. Logical operators

> Logical operators are typically used with Boolean (logical) values; when they are, they return a Boolean value. However, the && and || operators actually return the value of one of the specified operands, so if these operators are used with non-Boolean values, they may return a non-Boolean value. The logical operators are described in the following table.

10.Short-circuit evaluation 

As logical expressions are evaluated left to right, they are tested for possible "short-circuit" evaluation using the following rules:

<pre>false && anything is short-circuit evaluated to false.
true || anything is short-circuit evaluated to true.
</pre>

11.BigInt operators

Most operators that can be used between numbers can be used between BigInt values as well.

12.String operators

In addition to the comparison operators, which can be used on string values, the concatenation operator (+) concatenates two string values together, returning another string that is the union of the two operand strings.

13. Conditional (ternary) operator

The conditional operator is the only JavaScript operator that takes three operands. The operator can have one of two values based on a condition. 

14. Comma operator

The comma operator (,) evaluates both of its operands and returns the value of the last operand. This operator is primarily used inside a for loop, to allow multiple variables to be updated each time through the loop. It is regarded bad style to use it elsewhere, when it is not necessary. Often two separate statements can and should be used instead.

15. Unary operators
A unary operation is an operation with only one operand.

delete
The delete operator deletes an object's property. The syntax is:

<pre>delete object.property;
delete object[propertyKey];
delete objectName[index];
</pre>

16. Deleting array elements

> Since arrays are just objects, it's technically possible to delete elements from them. This is however regarded as a bad practice, try to avoid it. When you delete an array property, the array length is not affected and other elements are not re-indexed. To achieve that behavior, it is much better to just overwrite the element with the value undefined. To actually manipulate the array, use the various array methods such as splice.

<pre>typeof
The typeof operator is used in either of the following ways:

typeof operand
</pre>

To actually manipulate the array, use the various array methods such as splice.
<br
>
17. Relational operators

A relational operator compares its operands and returns a Boolean value based on whether the comparison is true.

in
The in operator returns true if the specified property is in the specified object. The syntax is: 

>>objectName instanceof objectType

18. instanceof

The instanceof operator returns true if the specified object is of the specified object type. The syntax is:

objectName instanceof objectType

19. Basic expressions

20. Grouping Operator

## Fifth Article: Functions

1. Function declarations
A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:

<pre>The name of the function.
A list of parameters to the function, enclosed in parentheses and separated by commas.
The JavaScript statements that define the function, enclosed in curly brackets, { /* … */ }.
</pre>

<pre>
Parameters are essentially passed to functions by value — so if the code within the body of a function assigns a completely new value to a parameter that was passed to the function, the change is not reflected globally or in the code which called that function.
</pre>

2. Calling functions
Defining a function does not execute it. Defining it names the function and specifies what to do when the function is called.


Calling the function actually performs the specified actions with the indicated parameters.

3. Function scope
Variables defined inside a function cannot be accessed from anywhere outside the function, because the variable is defined only in the scope of the function. However, a function can access all variables and functions defined inside the scope in which it is defined.

In other words, a function defined in the global scope can access all variables defined in the global scope. A function defined inside another function can also access all variables defined in its parent function, and any other variables to which the parent function has access.

4. Nested functions and closures

- The inner function can be accessed only from statements in the outer function.
- The inner function forms a closure: the inner function can use the arguments and variables of the outer function, while the outer function cannot use the arguments and variables of the inner function.

5. Multiply-nested functions

Functions can be multiply-nested. For example:

- A function (A) contains a function (B), which itself contains a function (C).
- Both functions B and C form closures here. So, B can access A, and C can access B.
- In addition, since C can access B which can access A, C can also access A.

6. Name conflicts

When two arguments or variables in the scopes of a closure have the same name, there is a name conflict. 

7. Closures

Closures are one of the most powerful features of JavaScript. JavaScript allows for the nesting of functions and grants the inner function full access to all the variables and functions defined inside the outer function (and all other variables and functions that the outer function has access to).

8. Predefined functions
JavaScript has several top-level, built-in functions:

- eval()
The eval() method evaluates JavaScript code represented as a string.

- isFinite()
The global isFinite() function determines whether the passed value is a finite number. If needed, the parameter is first converted to a number.

- isNaN()
The isNaN() function determines whether a value is NaN or not. Note: coercion inside the isNaN function has interesting rules; you may alternatively want to use Number.isNaN() to determine if the value is Not-A-Number.

- parseFloat()
The parseFloat() function parses a string argument and returns a floating point number.

- parseInt()
The parseInt() function parses a string argument and returns an integer of the specified radix (the base in mathematical numeral systems).

- decodeURI()
The decodeURI() function decodes a Uniform Resource Identifier (URI) previously created by encodeURI or by a similar routine.

- decodeURIComponent()
The decodeURIComponent() method decodes a Uniform Resource Identifier (URI) component previously created by encodeURIComponent or by a similar routine.

- encodeURI()
The encodeURI() method encodes a Uniform Resource Identifier (URI) by replacing each instance of certain characters by one, two, three, or four escape sequences representing the UTF-8 encoding of the character (will only be four escape sequences for characters composed of two "surrogate" characters).

- encodeURIComponent()
The encodeURIComponent() method encodes a Uniform Resource Identifier (URI) component by replacing each instance of certain characters by one, two, three, or four escape sequences representing the UTF-8 encoding of the character (will only be four escape sequences for characters composed of two "surrogate" characters).

- escape()
The deprecated escape() method computes a new string in which certain characters have been replaced by a hexadecimal escape sequence. Use encodeURI or encodeURIComponent instead.

- unescape()
The deprecated unescape() method computes a new string in which hexadecimal escape sequences are replaced with the character that it represents. The escape sequences might be introduced by a function like escape. Because unescape() is deprecated, use decodeURI() or decodeURIComponent instead.
