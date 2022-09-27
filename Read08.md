# First Article: Expressions and operators

## Expression: is a valid unit of code that resolves to a vavlue.

Type 1: have side effects
> Example: x = 7 assigning values

Type 2. purely evaluate
> Example: 2 + 4 using the operator to produces a value, but the ealuation does not produce any effect without being part of a bigger construct(for example variable declaration y = 2 + 4)

1. Assignment operators

> binary and unary operators

> assign to properties

<pre>
Name	                        Shorthand operator	Meaning
Assignment	                    x = f()	            x = f()
Addition assignment	            x += f()	        x = x + f()
Subtraction assignment	        x -= f()	        x = x - f()
Multiplication assignment	    x *= f()	        x = x * f()
Division assignment	            x /= f()	        x = x / f()
Remainder assignment	        x %= f()	        x = x % f()
Exponentiation assignment	    x **= f()	        x = x ** f()
Left shift assignment	        x <<= f()	        x = x << f()
Right shift assignment	        x >>= f()	        x = x >> f()
Unsigned right shift assignment	x >>>= f()	        x = x >>> f()
Bitwise AND assignment	        x &= f()	        x = x & f()
Bitwise XOR assignment	        x ^= f()	        x = x ^ f()
Bitwise OR assignment	        x |= f()	        x = x | f()
Logical AND assignment	        x &&= f()	        x && (x = f())
Logical OR assignment	        x ||= f()	        x || (x = f())
Logical nullish assignment	    x ??= f()	        x ?? (x = f())
</pre>

> Destructuring

Extract data from arrays or objects using a syntax that mirrors the construction of array and object literals.

> Evaluation and nesting
>> let, const, var

2. Comparison operators

Operator	                            Description	                                              
Equal (==)	                                Returns true if the operands are equal.	                   

Not equal (!=)	                            Returns true if the operands are not equal.	                

Strict equal (===)	                        Returns true if the operands are equal and of the same type. 

Strict not equal (!==)	                    Returns true if the operands are of the same type but not equal, or are of different type.	

Greater than (>)	                        Returns true if the left operand is greater than the right operand.

Greater than or equal (>=)	                Returns true if the left operand is greater than or equal to the right operand.

Less than (<)	                            Returns true if the left operand is less than the right operand.	

Less than or equal (<=)	                    Returns true if the left operand is less than or equal to the right operand.

3. Arithmetic operators

<pre>
Remainder (%)
Remainder (%)
Decrement (--)
Unary negation (-)
Unary plus (+)
Exponentiation operator (**)
</pre>

4. Bitwise operators

>Shift operators convert their operands to thirty-two-bit integers and return a result of either type Number or BigInt: specifically, if the type of the left operand is BigInt, they return BigInt; otherwise, they return Number.
<br>

5. Logical operators

>&&  
 ||
 !

6. BigInt operators

<pre>
// BigInt addition
const a = 1n + 2n; // 3n
// Division with BigInts round towards zero
const b = 1n / 2n; // 0n
// Bitwise operations with BigInts do not truncate either side
const c = 40000000000000000n >> 2n; // 10000000000000000n
</pre>

7. String operators

> In addition to the comparison operators, which can be used on string values, the concatenation operator (+) concatenates two string values together, returning another string that is the union of the two operand strings.
<br>

8. Conditional (ternary) operator

> The conditional operator is the only JavaScript operator that takes three operands. The operator can have one of two values based on a condition. The syntax is:

<pre>condition ? val1 : val2</pre>

<br>

9. Comma operator
> evaluates both of its operands and returns the value of the last operand. This operator is primarily used inside a for loop, to allow multiple variables to be updated each time through the loop. It is regarded bad style to use it elsewhere, when it is not necessary. Often two separate statements can and should be used instead.
<br>

10. Unary operators

>delete, typeof, void

11. Relational operators

>in, instanceof

12. Basic expressions

> this,new, super