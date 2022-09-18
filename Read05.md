# Reading Notes for Lab 4

## First Article: What is CSS

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

&nbsp;

## Second Article: How to Add CSS

### 1. Three ways to insert CSS

#### - External CSS

- External styles are defined within the <link> element, inside the <head> section of an HTML page:

- An external style sheet can be written in any text editor, and must be saved with a .css extension.

- The external .css file should not contain any HTML tags.

#### - Internal CSS

- The internal style is defined inside the <style> element, inside the head section.

#### - Inline CSS

- An inline style may be used to apply a unique style for a single element.

- To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.


&nbsp;

## Third Article: CSS Color

### 1. Definition and Usage

- The color property specifies the color of text.

- Tip: Use a background color combined with a text color that makes the text easy to read.

### 2. CSS Syntax

CSS Syntax
color: color|initial|inherit;

- Property Values

> color: Specifies the text color. 
> initial: Sets this property to its default value. 
> inherit: inherits this property from its parent element.

&nbsp;

## Fourth Article: CSS reference

### 1. Basic rule syntax

- Style rule syntax

<pre>
style-rule ::=
    selectors-list {
      properties-list
    }
</pre>

where:

<pre>
selectors-list ::=
    selector[:pseudo-class] [::pseudo-element]
    [, selectors-list] <br>

properties-list ::=
    [property : value] [; properties-list] <br>
</pre>

- Style rule examples

<pre>
strong {
  color: red;
}<br>

div.menu-bar li:hover > ul {
  display: block;
}<br>
</pre>

### 2. Index

### 3. Selectors

- basic selectors 

> Basic Selectors are fundamental selectors; there are the most basic selectors that are frequently combined to create other, more complex selectors.

>Universal selector *
>>Type selector elementname
>>Class selector .classname
>>ID selector #idname
>>Attribute selector [attr=value]

- Grouping selectors

>Selector list A, B
>>Specifies that both A and B elements are selected. This is a grouping method to select several matching elements.

- Combinators:
 are selectors that establish a relationship between two or more simple selectors, creating a complex selector

>> Adjacent sibling combinator A + B
Specifies that the elements selected by both A and B have the same parent and that the element selected by B immediately follows the element selected by A horizontally.

>> General sibling combinator A ~ B
Specifies that the elements selected by both A and B share the same parent and that the element selected by A comes before—but not necessarily immediately before—the element selected by B.

>> Child combinator A > B
Specifies that the element selected by B is the direct child of the element selected by A.

>> Descendant combinator A B
Specifies that the element selected by B is a descendant of the element selected by A, but is not necessarily a direct child.

>> Column combinator A || B Experimental
Specifies that the element selected by B is located within the table column specified by A. Elements which span multiple columns are considered to be a member of all of those columns.

- Pseudo

>> Pseudo classes :
Specifies a special state of the selected element(s).

>> Pseudo elements ::
Represents entities that are not included in HTML.

### 4. Concepts

1. Syntax and semantics

CSS syntax
At-rules
Cascade
Comments
Descriptor
Inheritance
Shorthand properties
Specificity
Value definition syntax
CSS unit and value types
CSS functional notations

2. Values

>Actual value
>Computed value
>Initial value
>Resolved value
>Specified value
>Used value

3. Layout

>Block formatting context
>Box model
>Containing block
>Layout mode
>Margin collapsing
>Replaced elements
>>Stacking context
Visual formatting model

4. DOM-CSS / CSSOM

>Major object types
>Document.styleSheets
>styleSheets[i].cssRules
>cssRules[i].cssText (selector & style)
>cssRules[i].selectorText
>HTMLElement.style
>HTMLElement.style.cssText (just style)
>Element.className
>Element.classList
>Important methods
>CSSStyleSheet.insertRule()
>CSSStyleSheet.deleteRule()

>Mozilla CSS extensions (prefixed with -moz-)
>WebKit CSS extensions (mostly >prefixed with -webkit-)
>Microsoft CSS extensions (prefixed with -ms-)

&nbsp;

## Fifth Article: Myers Web Reset Stylesheet

### CSS Tools: Reset CSS

1. Goal:
 
reduce browser inconsistencies in things like default line heights, margins and font sizes of headings, and so on.

