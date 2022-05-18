[Return to Course 201 Notes](https://KrisDunning.github.io/201/)

# Reading 07 - HTML Tables , Object Oriented Programming

*****

## HTML Tables

What is a table? A table represents information in a grid format. Made of rows and columns containing cells of information.  

Basic table structure:

- `<table>`- table element is used to create a table
- `<tr>`- indicates the start of each row. Uses `</tr>` closing tag
- `<td>`- each cell is represented with a td tag(table data). Uses `</td>` closing tag
- `<th>`- table heading. Like the `<td>` tag but represents the heading for either a column or a row.
- Each cell should be represented with either a `<td> or <th>` tag even if it contains no content to allow for proper styling
- `colspan`- column span attribute is used to indicate how many columns a cell should run across
- `rowspan`- row span attribute is same but for rows
- `<tfoot>`- on longer tables the `<th>` `<tbody>` and `<tfoot>` tags should be used for styling purposes. All have a closing tag associated

## Object Oriented Programming

### Object: Constructor Notation

~~~JS
var hotel = new Object();
hotel.name = 'hotel name';
hotel.rooms = 40;
hotel.booked = 25;
hotel.checkAvail = function(){
  return this.rooms-this.booked;
}
~~~

Objects can be update using dot notation., or square bracket notation
> hotel.name = "New name";  
> hotel['name'] = 'New name';

Object Constructors can be used to create many new objects with a ***Template***.

~~~JS
function Hotel(name,rooms,booked){
  this.name = name;
  this.rooms = rooms;
  this.booked = booked;
  this.checkAvail = function(){
    return this.rooms-this.booked;
  }
}
~~~

Names of constructors tend to capitolize first letters of the names unlike other functions. This helps remind programmers to uuse the **new** keyword when they create the object.  
We create **instances** of the object when using a constructor. The **new** keyword followed by a call to the functino creates a new object.  
> var holtonHotel = new Hotel('Holton',40,25);

To add a new property to a created object you can use dot notation. To remove a property use the `delete` keyword.
> hotel.pool=false;  
> delete hotel.pool;

If the property doesnt exist when using dot notation the property is added as a new key/value pair.  

An array is a special object containing key/value pairs but the key is the index and the value is the value at that index.  

Arrays can contain objects and objects can contain arrays creating a complex web of data. 

### Built in Objects

Browsers come with a set of built-in objects that represent things like the browser window and the current web page shown in that window. They act like a toolkit to create interactive web pages.  

Browser Object Model- Creates a model of the browser tab or window. The topmost object is the window object and its chil ibjects represent other browser features such as document, history,location(URL), navigator and screen.  

Document Object Model- The DOM creates a model of the current web page. The topmost object is the document object that represents the page as a whole. Its child objects represent other items on the page such as html, head, body, div, p, etc. 

Global JavaScript objects- The global objects do not form a single model. They are a group of individual objects that relate to different parts of the JavaScript language. Such as string, number, boolean, date, math and regex.  


## Things I want to know more about

factory format is good. industry uses? is class format better/clearer?


*****