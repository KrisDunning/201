[Return to Course 201 Notes](https://KrisDunning.github.io/201/)

# Reading 08 - CSS Layouts

*****

## Layout History

Early CSS layouts were based on the HTML `<table>` elements. CSS's adoption by browsers in the late 90's opened the door to developers being able to completely control the look of a website without touching the HTML.  

## Display Property

`display` property does two things  

- 1st- determines if the box it is applied to acts as inline or block
- 2nd- determines how an elements children should behave. for example the `disply:flex` makes a block level box and also converts children to flex items.

There are two main layouts that create rules for multiple elements `flexbox` and `grid`. They share similarities but are designed to solve different layout problems.  

## Flexbox

Flexbox is a layout mechanism for one-dimensional layouts. Across a single axis, either horizontal or vertical. By default flexbox will align the elements children next to each other in the inline direction and strecth them in the block direction so they are all the same height.  

Items will stay on the same axis and not wrap when they run out of room but will instead try to squash onto the same line as each other.  

This behaviour can be changed using the `align-items`, `justify-content` and `flex-wrap` properties.  

The `flex` property can control how the chilren behave in a flex container. It is a shorthand for `flex-grow`, `flex-shrink` and `flex-basis`.  

Develops provide these low-level rules to tell a browser how the layout should change by content and viewport dimensions. This makes it useful for responsive web design.  

## Grid

`grid` display is similar to flexbox but is designed to control multi-axis layouts.  

Grid enables you to write rules on an element that has `display:grid` and introduces a few promitives for layout styling. `repeat()` and `minmax()` functions and a new unit the `fr` unit which is a fraction of remaining space.  

The `grid-row` and `grid-column` properties instruct the element to span a certain length (ex. 1/3 or 1/4).  

`Inline-block` makes inline elements respect block margin and padding on an inline element. 

`Float` property instructs an element to "float" in a direction specified, left,right,inherit etc.  

## Multicolumn layout

If you have a long list of elements such as a list of countries it can cause a lot of scrolling. Using CSS multicolumn you can split this into multiple columns.

> .countries{
>column-count: 2;  
>column-gap: 1em;  
> }  

Instead of setting the number of columns that the content is split into you can also define a minimum desired width using `column-width:`. As more space is available in the viewport, more columns will automatically be created.  

## Position

`position` property changes how an element behaves in normal flow of a document. The position display options are:

- relative
- absolute
- fixed
- sticky
- static (default)

Relative- makes it the containing block of any child element with `position:absolute`. This means that its child will now be repositioned ot this elemnt instead of the topmost relative paren by using `position:absolute`.  

Absolute- This breaks the element out of the current document flow which means you can position the element using top,right, bottom and left in its nearest parent. Also all of the content surrounding an absolute element reflows to fill the remaining space left by the element.  

position:fixed- behaves similarly to absolute with its parent being the root `<html>` element. Use top,left,bottom,right to position relative to the html element. 

sticky- anchored and fixed aspects of `fixed`and as the viewport scrolls this element will retain its anchored position according to its top,right,bottom,left values.  

## Things I want to know more about

flexbox and grid, especially mixing all positions/displays.  
can i make something relative to a gridbox?

*****