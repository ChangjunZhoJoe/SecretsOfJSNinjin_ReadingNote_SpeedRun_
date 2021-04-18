# Guys Welcome! This is the note I wrote when I speedrun the book!
## Mark April 16 2020, I started speed running the book.

(TO-DO: Why I speed run this book?)  
## Day 1
######   Browser three bros: HTML JS CSS.  Browser three bros: HTML JS CSS.  
######   HTML is like the blueprint of DOM tree in browser. Note the DOM does not have to be 100% built like HTML.  
######   Two phase when loading DOM: 1 Parsing HTML 2 Run Javascript. 
######   Browser read HTML line by line when constructing DOM. It runs the javascript when encounter <script> tag.
######   Javascript has access to 'window', which represents the website that the js runs in. 'Document' is a element of 'window'.  
######   Event queue is a nice feature. The queue is operated in browser not js. I think it's FIFO queue.  
######   Not only JS can register events in the event queue. But also the browser (incoming network traffic) and the user(click) register events.  
  
## Day 2
######   Function context. There is always one "window" context. "this" keyword inside a function refers to its context.
######   Ways of defining functions. function declaration. arrow function. function as method. "new" keyword. 
######   "arguments" and "this" are implicitly passed to function as arguments.
######   "arguments" contains all the arguments passed into a function.
######   "arguments" is not an array. 
######   The values in "arguments" entries are shadow-copy of real arguments, so changing one will reflects on others.
######   Use of "new" + function as object initializer. Use "this" to refer to the calling object.
######   Function context depends on function invocation.
######   Arrow functions uses the context when its created, if not explicitly changed.
######   TBH try don't use this, its chaotic.
