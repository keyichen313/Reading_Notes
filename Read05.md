# Reading Notes for Lab 4

## First Article

### 1. What is CSS?

CSS (Cascading Style Sheets) allows you to create great-looking web pages, how documents are presented to users.

&nbsp;

Browser Defaults

- the browswer will style HTML documents using an internal stylesheet.

- Using CSS, you can control exactly how HTML elements look in the browser.

&nbsp; 

### 2. What is CSS for?

- A document is usually a text file structured using a markup language--HTML is the most common markup language.

- presentinga document to a user means converting it into a form usable by your audience. The Browsers/user agents are designed to present documents visually.

### 3. CSS syntax

- CSS is a rule-based language- you define the rules by specifying groups of styles that should be applied to particular elements or group of elements on your web page.

- CSS rule opens with a ***selector***, which select the HTML element that we are going to style.

<pre>
example:
hi{
    color: red;
    Font-size: 5em;
}
</pre>

- Inside the braces will be one or more ***declarations***, which take the form of property and value pairs.

<pre>example: color and font-size are properties, red and 5em are values.
</pre>

### 4. CSS Modules

As there are so many things that you could style using CSS, the language is broken down into modules. You'll see reference to these modules as you explore MDN. Many of the documentation pages are organized around a particular module.

### 5. CSS Specifications

All web standards technologies (HTML, CSS, JavaScript, etc.) are defined in giant documents called specifications (or "specs"), which are published by standards organizations (such as the W3C, WHATWG, ECMA, or Khronos) and define precisely how those technologies are supposed to behave.

- New CSS features are developed or specified by the CSS working group
- they are intended for engineers to use to implement support for the features in user agents, not for web developers to read to understand CSS. 

### 6. Browser support information

- The browser support status is shown on every MDN CSS property page in a table named "Browser compatibility". The browser support status is shown on every MDN CSS property page in a table named "Browser compatibility". 

- Based on your requirements, you can use the browser compatibility table to check how this property is supported across various browsers, or check if your specific browser and the version you have support the property, or if there are any caveats you should be aware of for the browser and version you are using.



