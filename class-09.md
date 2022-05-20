[Return to Course 201 Notes](https://KrisDunning.github.io/201/)

# Reading 07 - HTML Tables , Object Oriented Programming

*****

## Forms

Many different forms available to take information from a user and send it to a server.  

- Input-text- A single line text input
- Input-password- A text box with the characters blocked out. Not secure!
- Text Area- a multi-line text input
- Radio Button- Allows users to pick just one of multiple options
- Checkbox- Allows users to select and unselect one or more options
- Drop down list- Also known as a select box. Allows users to select one option from a drop down list
- Multiple select box- Can allow users to select multiple options from this list by adding the multiple attribute.
- Input-File- Allows users to upload a file
- Submit Button- Used to send a form to the server
- Image Button- If you want to use an image for the submit button
- Button- Allows users more control over how their button appear
- Input-hidden- The form controls are not shown on the page but allows page authors to add values to forms the users cannot see
- Input-date- Create a date input
- Input-email- Asks for an email and will do some input validation
- Input-url- Allows and semi-validates for url input
- Input-search- Single line text box for search queries

Labels- Each form should have its own label element as this is useful for accessablity.  

For- the for attribute states which form control the label belonds to 

> `<label for="address">Address</label>`

Fieldset- You can group related form controls together inside the fieldset element. Most browsers show a line around the edge to show how they are related

Legend- This element shows a caption which helps identify the purpose of that group of form controls

> `<fieldset>`  
> `<legend>Contact Details</legend> </fieldset>`

## List, Table and Form styling

- List-style-type- CSS property that controls the list "marker" or the bullet point style. disc,circle,square for ul. decimal, lower-alpha ,lower-roman etc/
- list-style-image- specify an image to be used for the marker. CSS property with value of url("img.png")
- list-style-position- value of outside or inside. determines if the marker is left or inside of the list text box
- list-style- shorthand for list-style properties
- Empty-cells- empty-cell property can show or hide borders for empty table cells
- Border-Spacing- borders are detached from each other
- Border-collapse- borders collapse into a single border where possible

## Events

When interacting with a web page the browser will send up a signal saying "Hey this thing is happening". These are called events.  
When an event fires it can be used to trigger an execution of code.  

Event Handlers  

- DOM Event Handlers- Can only attach one function to an event
- Event Listeners- introduced in DOM level 2, now the favored way to handle events. Allows one event to trigger multiple functions. 



## Things I want to know more about

event listeners usage for windows and not just DOM

*****
