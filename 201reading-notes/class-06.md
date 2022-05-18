[Return to Course 201 Notes](https://KrisDunning.github.io/201/)

# Reading 06 - JS Object Literals, DOM Manipulation

*****

## Objects

Objects group together a set of variables and functions to creats a model of something you would recognize from the real world.  

In an object, variables become known as properties. `Properties` tell us about the object such as its name or number of things it has.  

In an object, functions become known as methods. `Methods` represent tasks that are associated with the object.  

Properties and methods have a name and a value. In an object the name is called a `key`. An object can not have two keys with the same name. The value of a property can be a string, number, Boolean, array or even another object. The value of a method is always a function.  

**Literal Notation:** The easiest and most common way to create objects is call literal notation. (there are many ways to create objects)  

~~~~JS
var hotel = {
  name: 'Hotel 88',
  rooms: 88,
  booked: 42,
  checkAvailable: function (){
    return this.rooms-this.booked;
  }
}
~~~~

In the `checkAvailable()` method the **this** keyword is used to indicate that it is using the rooms and booked properties of this object. 

**Accessing An Object:** to access a property or method of an object you use the name of the objects followed by a period then the name of the property or method you want to access. This is called `dot notation`.  

> var hotelName=hotel.name;

You can also access properties (but not methods) using square bracket syntax.  

> var hotelName=hotel['name'];

## DOM Manipulation

The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.  

DOM is neither part of HTML nor JS, it is its own separate set of rules and is implemented by browser makers.  

The DOM covers two primary areas:

- Making a model of the HTML page
  - DOM specifies the way a browser structures the mode using a **DOM TREE**. The DOM is called an object model because the tree is made of objects.
- Accessing and changing the HTML page
  - DOM also defines methods and properties to access and update each object in this model.

DOM's are API's (app. programming interface). API's let programs and scripts talk to each other.  

Accessign the DOM tree invovles two steps:

- Locate the nod that represents the element you want
- Use its text content, child elements and attributes

A `node` on the tree is used interchangably with the element it represents.  

When we set a variable to an element node on the DOM tree we are saving a reference to the nodes location on the tree. This is known as **caching** the selection.  

DOM queries will return a `nodelist` if the method *can* return more than one node.  

Methods that return a single element node:  

- `getElementById('id')`
- `querySelector('css selector')`

Methods that return one or more elements(nodelist)

- `getElementsByClassName('class')`
- `getElementsByTagName('tag name')`
- `querySelectorAll('css selector')`

DOM methods can also be used on element nodes withing the page to find descendants of that node.  

Nodelists look like arrays and are numbered like arrays but they are actually a type of object called a `collection`.  

When we make a element selection we can create a nodelist. Nodelists come in two varietys:

- Live Nodelost- when your script updates the page the nodelist is updated at the same time. Methods beginning with `getElementsBy...` return live nodelists.
- Static Nodelists- When your script updates the page this nodelist is not updated to reflect the changes made. The methods beginning with `querySelector...` return static node lists.

There are two ways to select an element from a nodelist:

- `item()` method- var firstItem=elements.item(0)
- array syntax- var firstIem=elements[0]

## Traversing the DOM

When you have an element node you can select another element in relation to it using these five properties, also known as traversing the DOM.

- `parentNode`- property that finds the parent node
- `previousSibling`- property that finds previous sibling( null if not found)
- `nextSibling`- property that finds next sibling (null if not found)
- `firstChild`- property that finds first child (null if not found)
-`lastChild`- property that finds last chile (null if not found)

Whitespace- most browsers treat whitespace between elements (such as spaces or carriage returns) as a text node and as such the above properties may return different elements in different browsers. The jQuery library rose to popularity because it bypassed this issue with DOM traversing.  

Accessing and replacing a text node with `nodeValue`

>var item=document.getElementByID('itemOne')
>var itemText=item,firstChild.nodeValue;
>itemText=itemText,replace('oldtext', 'newtext');
>item.firstChild.nodeValue=itemText;

## Things I want to know more about

industry standard for best use case of object literals

is getElementById the standard window into DOM?

*****
[Return to Course 201 Notes](https://KrisDunning.github.io/201/)
