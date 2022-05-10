[Return to Course 201 Notes](https://KrisDunning.github.io/201/)

# Reading 01- Intro to HTML and JavaScript

*****

## Intro

 What is the web and how do we access it? We use *web browsers* to access web sites. Different companies create different browsers such as Apples Safari or Microsofts Edge. When we ask the web browser to view a website, the browser asks a special computer called a *web server* who hosts the web site. Websites currently use HTML5 and CSS3 to create basic websites.  

## Chapter 1

 HTML lays out the content of a page, a structure. The layouts used in web pages often harken back to newspapers or magazines. The header element h1 resembles the headline of a newspaper. The body and paragraphs follow common convention. HTML uses *tags* and *attributes* to define the meaning and intent of the code.  

 To create a web page for yourself use a text editor such as Notepad++ or TextEdit. Simply start a file. Add some HTML and save the file as a xxxx.html file extension. Then open the file with the browser.  

## Chapter 8

There have been several iterations of HTML and because of the changes over the years we use `!DOCTYPE=HTML5` in our xxxx.html files to tell the browser which HTML we intend to use.  

Another useful tool to use is the code comment.  
> `<!-- comment -->` This code snippet is used to leave a comment that is not visible to the user of a web page.  

Additionally there are `attributes` which can be assigned to HTML `elements` that allow them to be uniquely identified.  
> `id="text` and `class=text` are used to allow CSS to be applied to specific elements on a web page. Id's need to be unique but there can be multiple elements that share a class identifier. This allows changes in 1 specific location or changes to a specific subset of multiple elements.  

`<iframe>` are little windows on web pages. They require a `<src>` to specify the URL of the page to show in the frame and a `height` and `width` to set the size of the window.  

HTML elements are generally displayed using one of two defaults. `Block` and `Inline`.  

Block elements (ex. h1,p,ul,li) will start on a new line when displayed on a web page.  

Inline elements (ex. a, b, em, img) continue on the same line as the previous element.  

We can use HTML elements to choose which display method we want by using `<div>` elements for blocks and `<span>` elements act like inline elements. 

## Chapter 17

New HTML5 layout elements have been introduced to reduce the usage of generic `<div>` and `<span>` elements.  

`<header>` and `<footer>` have been added to be used for a commonly re-used space at the top or bottom of the page. Such as a navigation bar or contact information.  

`<nav>` is an element that is used to contain the major navigational blocks used for site navigation. Not all links need the attribute.  

`<article>` is an element that acts as a container for a section of a page that can stand on its own. Articles can even be nested within each other.  

`<aside>` is an element that has two uses. When inside an `<article>` it should contain related material that is not essential to its meaning, like a glossary for example. When outside an article it acts as a container for content realated to the page as a whole. Such as a list of posts or links to other pages or a search box.  

`<section>` is an element that groups related content together and generally has its own heading. May be used to contain articles or may be used to break up a long article into subsections.  

`<fig>` and `<figcaption>` are used to contain any content that is referenced from the main article, often an image but not necessarily (ex. Videos, graph, Diagram, Supporting Text). The fig caption attaches a caption to the figure.  

## Chapter 18

The design process for a website starts with who your target audience is. Some questions to ask are:

- What is the age range of users?
- Does your site appeal to men?women? what mix of both?
- Which country are users coming from?
- What device do they use to access your site?

These questions and others can help guide the design of the page and increase its chance to succeed.  

Now that you have the who, you can investigate the why. What are their *motivations* for coming to the site. Do they have a *specific goal* for coming to the site?  

What information do your users need to achieve their goals? Present the most important information up front in a succinct manner. Offer supporting information should the user require it.  

How often do you expect users will come to the site? News sites are updated multiple times in a day, roofing replacements less so.  

A tool used to visualize the structure of the site is a `site map`. It's like a flow chart of where each individual page on a site should sit in relation to the other pages. Think family tree.  

Wireframes are a simple sketch of the key information that goes on each page and shows a heirarchy of information. Keep this simple, no colors, fonts, images, etc. Save that for the site design phase.  

The design phases goal is to communicate information to the user. We need to prioritize and organize the information so that it is digestible.  

## JS Chapter 1

A script is a series of instructions not unlike a baking recipe. Scripts can use only a subset of their code at a given time and can check the current browser situation to perform only the set of steps if it is appropriate.  

To write a script you need to first set a goal and then list the steps needed to achieve that goal. Then go in and add code to fill out the steps. 

In computer language we can model the world around us using Objects(things) and Properties(chracteristics). Events are "flags" that we can identify and respond to using our scripts. Methods() are how we interact with an Object. A openDoor() method could be used to open a car objects door.  

Web browsers are programs built using objects. A window object (browser) can deliver the document object(web page) to the user. This is the origin of the ***Document Object Model(DOM)***.  

## Things I want to know more about  

- Event handling in JS scripts.
- DOM manipulation
- CRUD operations using JS and either JSON or a DB

*****

[Return to Course 201 Notes](https://KrisDunning.github.io/201/)
