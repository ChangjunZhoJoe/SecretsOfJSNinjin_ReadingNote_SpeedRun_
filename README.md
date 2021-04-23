# Guys Welcome! This is the note I wrote when I speedrun the book 'Secrets of the Javascript Ninja' 🎉 🍸
## Mark April 16 2020, I started speed running the book.

(TO-DO: Why do I speed run this book?)  
## Day 1 History and introduction of JS.
######   Browser three bros: HTML JS CSS.  Browser three bros: HTML JS CSS.  
######   HTML is like the blueprint of a DOM tree in a browser. Note the DOM does not have to be 100% built like HTML.  
######   Two phases when loading DOM: 1 Parsing HTML 2 Run Javascript. 
######   Browsers read HTML line by line when constructing DOM. It runs the javascript when encounter <script> tag.
######   Javascript has access to 'window', which represents the website that the js runs in. 'Document' is an element of 'window'.  
######   Event queue is a nice feature. The queue is operated in browser not js. I think it's a FIFO queue.  
######   Not only JS can register events in the event queue. But also the browser (incoming network traffic) and the user(click) register events.  
  
## Day 2 Function introduction
######   Function context. There is always one "window" context. "this" keyword inside a function refers to its context.
######   Ways of defining functions. function declaration. arrow function. function as a method. "new" keyword. 
######   "arguments" and "this" are implicitly passed to function as arguments.
######   "arguments" contains all the arguments passed into a function.
######   "arguments" is not an array. 
######   The values in "arguments" entries are shadow-copy of real arguments, so changing one will reflect on others.
######   Use of "new" + function as object initializer. Use "this" to refer to the calling object.
######   Function context depends on function invocation.
######   Arrow functions use the context when it's created, if not explicitly changed.
######   TBH try don't use this, it's chaotic.
  
Took a 3 days break for final exams :>  I thought I could finish this book in a week. But here I am, done 50% after a week with exams and stuff. I need to finish this book in time to work on my other ideas.


## Day 3 Closure and scope. ---- execution context, lexical env and (let, var, const)
######   First of all, there is an execution context. It's like a stack of executing functions ordered by scope. The one at the bottom is always the 'window', the js boss. The more up it goes, the less scope it gets. 
######   Functions, blocks (ex. for loop) can all be put into the execution context.
######   A Lexical environment is a place (like a stack) to store the information of objects inside each closure in order to track them. It's used when determining the scope of any object.
######   Program go search for an object identifier in the lexical env start from the top, if not found, it goes to the closest outer lexical env. And it kept going until it searched the 'window' env and had no results. 
######   Unlike private or public in java. Identifier declared by var is assigned to the closest function lexical env, it skips block (ex. for loop). 
######   Let assign an identifier to the closest lexical env no matter block or function. 
######   Const's scope is the same as Let but, the identifier could not be completely reassigned.
######   JS scans the declared function identifiers excluding arrow functions at the first time it reads the js file. That's why we could use the function that has yet to be declared. 

## Day 4 Generators and promises.    Promise Promise.all Promise.any catch 
######   Generators are a function that could be suspended and resumed. Do *function func_name(){} when you declare it. 
######   Promises are syntax sugar built based on generators. 
######   ES6 introduces async function(){ await another_func_name() }. It's like multiprocessing. Though js is a single thread language.
######   Good syntax sugar Promise Promise.all Promise.any catch. Remember them and you will use them. 

## Day 4 prototyping and fake object oriented programming in javascript. 
######   Prototype is like a parent blueprint.  
######   Prototypes come with any objects(functions). It's auto-attached to the object when it's created. 
######   By initializing obj with a new keyword. By var objBanana = new PenCup(); you initialize objBanana with everything from PenCup's prototype. 
######   By var objBanana = new PenCup(); objBanana.prototype and PenCup.prototype refer to the same prototype in memory. 
######   You can change the prototype by just assigning it like objBanana.prototype = anotherPrototype. But it's stupid to do it.
######   I won't mention some practical pitfalls when using prototypes. Let's use them less, it's safer this way.
######   Coming with ES6, class, inheritance are coming to js. They are all built with prototyping. We just lost another excuse to use a prototype! (I don't like prototyping, it's humanly-designed-complicated). 
######   Use Object.defineProperty(obj,propertyName, {specifications}) to define a property with certain rules like enumarable. writable etc. 


## Day 5 Controlling access to objects --- Getter Setter Proxy
######   You can use Getter and Setter to define the action when retrieve and modifying an 'object liked function'. 
######   Use getter and setter with constructor function to mimic 'private' variables. 
######   Proxy is a way to gain completely control over an object. Get, set and called(as a function) and more could be intercepted by proxy. 
######   Proxy is much slower (dozens of times) than not using it.



