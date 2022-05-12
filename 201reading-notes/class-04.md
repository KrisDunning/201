[Return to Course 201 Notes](https://KrisDunning.github.io/201/)

# Reading 04- HTML Links, JS Functions, and Intro to CSS Layout

*****

## Links

Links are the defining feature or the web. They alllow browsing or *surfing* of the web.  
Links can be used to link to other websites, one page to another on the same site, from one part of a page to another part and even open a new browser or open an email program.  
Links are created using the `<a>` element. The href attribute sets the destination of the link. The text between the open and closing tag is the clickable link.  
>ex. `<a href="website.com">Click Here for Website</a>` 

For linking to pages on the same site you can use relative linking.  

- same folder - "page.html"
- child folder - "childfolder/page.html"
- grandchild folder - "child/gchild/page.html"
- parent folder - "../page.html"
- grandpparent folder - "../../page.html"

Linking to specific part of the same page is done by utilizing the #id property. ex. `<a href="#topofpage">`  
Linking to another sites specific id is possible too.  
ex. `<a href="https:www.otherpage.com/#footer">`

## CSS Layout

Building Blocks :  
Block-Level Elements start on a new line (h1,p,ul,li)  
Inline Elements flow in between surrounding text (img,b,i)  

Containing elements or parent elements are when one block level element contains another block element.  

Positions:  

- Normal Flow - default behavior. elements start on a new line.
- Relative - Removes from normal flow, can be placed top, right, bottom, left of where it would have been.
- Absolute - Positions in realtion to its containing element. Removed from normal flow. Moves if user scrolls up or down.
- Fixed - Like absolute except is positioned in relation to the browser window not the containing element and does not move when the page scrolls.
- Floating - Out of normal flow and can be positioned within containing element and it becomes a block level element which other content can flow. Use z-index to control which shows on top.

## Modern Screen Information

Screen Sizes  
Sizes can vary from the smallest phone screens, to tablets, to laptop, to giant 27 in. + monitors.  

Screen Resolution  
Resolutions can be anywhere from 720x480 up to 4k. The higher the resolution, the smaller the text. Even phones can have a higher resolution than some monitors.  

Page Sizes  
Because of variety of screen sizes and resolutions web designers create pages of around 960-1000 pixels wide. The screen area seen without scrolling is called "**above the fold"**. In general try to get the most important information in the top 570-600 pixels (height from top of page).  

## Layout Grids

A commonly used layour grid is the **"960 pixel grid"**. It consists of thick vertical lines with consistent proportions and spaces between items to help create a progessional looking design.  

## JS Functions

Functions let you group a series of statements together to perform a specific task.  

>function funcName()  
>{  
>statements that do stuff  
>}

Rule number one. Functions only do something when called!  
`funcName();`  

Parameters and arguments:  
There is a subtle difference though they are often used interchangably. Parameters are the variables that the function receives and are declared in the function declaration. Arguments are the variables that are sent to the function during the function call.  



*****

[Return to Course 201 Notes](https://KrisDunning.github.io/201/)
