[Return to Course 201 Notes](https://KrisDunning.github.io/201/)

# Reading 13 - Local Storage

*****

## History

Native client apps have historically been better at offering persistent local storage.  

Typically apps have offer an abstraction layer for storing and retrieving data. You can additionalls embed your own database, invent your own file format or many other solutions.  

Historically web applications have had none of these. Cookies have been available for many many years but they are included with every HTTP request so they slow down sites, are unencrypted and limited to 4 KB of data.  

Ideally web apps want a lot of storage space, on the client, that persists beyond a page refresh and isn't transmitted to the server.  

"HTML storage" or now a specification of its own known as **Web Storage**. It may also be known as "local storage" or "DOM storage".  

## HTML5 Storage

So what is HTML5 storage? It is a way for web pages to store name key/value pairs on within the clients web browser and it will persist even if the user navigates away from the page or exits the browser.  

In JavaScript you can access the data through the `localStorage` object on the global `window` object. Before using you should detect whether the browser supports it.  

You can store data based on a named key and can retrieve data with that same key. The named key is a string. The data can be any type supported by JavaScript. However the data is stored as a string as well. You will need to coerce your values into the expected datatypes upon retrieval.  

> getter - getItem('key');
> setter - setItem('key',data);

If getting a non-existent key, get a `null` instead of an exception.  
If setting to an alraedy named key, it will "silently" overwrite its value.  

## Things I wish I knew more about

 webDB? "SQLite" but out of date? IndexedDB API? uses its own methods but is it supported well on browsers?

*****
