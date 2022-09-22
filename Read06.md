# Reading Notes for Lab 6 JavaScript

## First Article: JavaScript

### 1. Definition

> JS is a lightweight, interpreted, or just-in-time compiled programming language with first-class functions.

> scripting language for webpage, but many non-browser environment also use it.

> the standards for JavaScript are the ECMAScript Language Specification(ECMA-262) and the ECMAScript Internationalization API specification

#### JavaScript First Steps

> Beginning

- Variables
- Numbers and operators
- Strings
- Useful string Methods
- Arrays

> Intermediate

1. Framework

2. Overview

3. data structures

4. Equality comparisons and sameness

5. Closures

> Advanced

1. Inheritance and phototype chain

2. strict mode

3. JavaScript typed arrays

4. Memory Management

5. Concurrency model and Event Loop


## Second Article: Introduction: Basic Output

- The language itself. This is fairly standard among the various environments, both in the various browsers and in the various server-side environments.<BR>

- The DOM API - how the language can interact with the various parts of a web page while in the browser. While in this respect the various browsers are getting closer to each other they still differ. Several libraries, most prominently JQuery, is trying to provide a unified API(Application Programming Interface).<BR>

- The server API (or just API) provided by Node.js or one of the other server-side systems.

1. Editor or IDE

2. Embed or Include

    Embed: add <script> Your JavaScript Code Here</script> inside HTML

3. Input Output

>. Alert

>. Document.Write

>. Console.log

## Third Article: JavaScript Input with Prompt and Confirm

### Prompt

1. examples/js/prompt.html

<pre>
<script>
 
var name = prompt("Your name:", "");
document.write("Hello ", name);
 
</script>
</pre>

2. Confirm

<pre>
<script>
 
if (confirm("Shall I print Hello World?")) {
    document.write("Hello World");
} else {
    document.write("OK, I won't print it.");
}
 
</script>
</pre>

## Fourth Article: JavaScript Variables

1. Variables are containers for storing data

2. Always declare JavaScript variables with var, let, or const

3. If you want a general rule: always declare variables with const. If you think the value of the variable can change, use let.

4. Identifiers: all variables must be identified with unique names. (case sensitive)

5. The Assignment Operator is =; equal to operator is ==

6. Data Types:

>> strings: double or single quotes

>> numbers: without quote

7. One statement, many variables

8. Value = undefined

9. Re-declaring JavaScript Variables

>> you can re-declare variable with var, but not with let or const

10. JavaScript Arithmetic

>> if you add strings inside the arithmetic, the strings will be concatenated.

11. Dollar Sign: as a letter

12. Underscore: as a letter.