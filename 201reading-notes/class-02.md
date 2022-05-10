[Return to Course 201 Notes](https://KrisDunning.github.io/201/)

# Reading 02 - Basics of HTML CSS and JS

*****

## Ch.2 HTML

Markup is adding tags to the contents of the page. There is *structural* markip and *semantic* markup. Structural markup is for elements that you can use to descrube both headings and paragraphs. Semantic markup provides extra information such as emphasis on a word or meaning of acronyms.  

Headings come in 6 levels.  
Paragraphs are block elements that are used to contain content.  
Bold, Italic, Superscript and Subscript allow text to be modified for display purposes.  `<b> <i> <sup> <sub>`.  
Line breaks `<br />` can be used to enter a new line.  
Horizontal Rules `<hr />` can be used to show a visual break between content.  
Both these are called *empty tags* and only have an single set of brackets.  

Some semantic markups are as follows:

~~~~~ HTML
<strong> - content has strong emphasis and defaults to bold.
<em> - indicates emphasis and defaults so italic.
<blockquote> - used for longer quotes. <p> should still be within a BQ element.
<q> - quote element that sit within paragraphs.
<abbr> - for abbreviations or acronyms. `abbr title="professor">Prof</abbr>.
<cite> - when referencing a piece of work such as a book or movie. Defaults to italics.
<dfn> - definition of a term or jargon. A <dfn>Black Hole</dfn> is a gravity pit in space. Some browsers default italic but not all. 
<address> - used to contain contact details of the page author. May contain address, phone number or email. 
<ins> / <del> - used to show content that has been added or deleted from the document. Insert defaults to underline. Delete defaults to strikethrough. 
<s> - strikethrough. indicates content no longer accurate but should not be deleted. i.e. an old sale price.

~~~~~

## Ch. 10 CSS

CSS works by associating rules with HTML elements. CSS rules contain 2 parts: a *selector* and a *declaration*.  

CSS declarations sit inside curly brackets (`{ }`) and contain 2 parts themselves. *Properties* and *values*.  

Using external CSS:

~~~ HTML
<link href="css/style.css" type="text/css" rel="stylesheet"/>
link is the element in HTML used to tell browser where to find the CSS. 
href is the file path to the CSS file.  
type is the attribute specifying the type of document linked and should be text/CSS.  
rel is the relationship between HTML and the linked file. 
You can link more than 1 CSS file if needed.
~~~

Using Internal CSS:

~~~ HTML
  <style type="text/css">
  body{ color:red;}
  p{ color:blue}
  </style>

CSS rules can also be included within HTML files. They rules must exist within the `<style>` tags. External stylesheets are the preffered method of utilizing CSS.  
~~~

CSS selectors allow you to specify which elements you want to style with the CSS rules.  

CSS selectors are case sensitive and must match element names and attribute values exactly.  

CSS rules work in a top down manner and can be inherited from their parent element.  

## JS Ch. 2 - JavaScript Basics

A script is a series of instructions that a computer follows one-by-one. Each step of the instructions are called statements.  

Comments should explain what your code does (or why). `/* comments here */`.  

Variables are containers that store data.  

~~~JS
How to declare and assign a value to variables:

let food = "pizza";

let is the variable keyword, food is the variale name, the equal sign is the assignment operator and the variable value is pizza.
~~~

There are 7 types of variables in JS:

- numeric- holds numeric data
- string- holds text values
- boolean- either true or false
- arrays
- objects
- undefined
- null

## JS Ch. 4 Decisions and Loops

To control the flow of data we can use evaluations, decisions and loops. First we determine a condition to be checked. Then evaluate the data to see if it meets a condition and then move on based on the conditional evaluation outcome.  

Comparison operators and logical operators can be used to evaluate the conditions. Comparison operators are like greater than or less than or equal to. Logical operators are and (&&) or(||) not(!).  

We can use if and if else statements to check conditions as well. There is also the switch statements which allows for multiple cases to be evaluated against the value provided.  


## Things I want to know more about

- hCards for `<address>` element. Still used? Worth learning?

- CSS selector cheat sheet. (HTML book page 238)

*****

[Return to Course 201 Notes](https://KrisDunning.github.io/201/)
