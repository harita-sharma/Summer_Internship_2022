<b>Q1. What is NodeJS? </b>

Node. js (Node) is an open source development platform for executing JavaScript code server-side. Node is useful for developing applications that require a persistent connection from the browser to the server and is often used for real-time applications such as chat, news feeds and web push notifications.
<li>Node.js is an open source server environment.</li>
<li>Node.js is free</li>
<li>Node.js runs on various platforms (Windows, Linux, Unix, Mac OS X, etc.)</li>
<li>Node.js uses JavaScript on the server.</li>
<br>
<b>Q2. What is V8 Engine? </b>

<br>

V8 is a C++-based open-source JavaScript engine developed by Google.
V8 is the JavaScript engine i.e. it parses and executes JavaScript code.It provides a runtime environment for the execution of JavaScript code. The best part is that the JavaScript engine is completely independent of the browser in which it runs.

<b>Q3. What is Event Loop in NodeJS.</b>
<ul>
<li>  Event loop is an endless loop, which waits for tasks,       executes them and then sleeps until it receives more tasks.</li>
<li>The event loop executes tasks from the event queue only when the call stack is empty i.e. there is no ongoing task.</li>
<li>The event loop allows us to use callbacks and promises.</li>
</ul>

<b>Q4. What is the use of tsconfig.json file?</b>

tsconfig.json file is a file of JSON format which allows us to point the root level files and different compiler options to setup that require to compile a TypeScript based projects. The existence of this file in a project specifies that the given directory is the TypeScript project folder root. 

The tsconfig.json file mainly consists of the information for the following:

<li>CompilerOptions</li>
<li>CompileOnSave</li>
<li>Files</li>
<li>Include</li>
<li>Exclude</li>
<br>
<b>Q5. What are the methods provided by 'fs' module to manipulate files?</b>

<br>

With Node.js, you can programmatically manipulate files with the built-in fs module. The name is short for “file system,” and the module contains all the functions you need to read, write, and delete files on the local machine.

you will use the fs module to read a file created via the command line, create and write to a new file, delete the file that you created, and move the first file into a different folder. 

<li>Reading Files with readFile()</li>
<li>Writing Files with writeFile()</li>
<li>Deleting Files with unlink()</li>
<li>Moving Files with rename()</li>
<br>
<b>Q6. What is API?</b>

<br>

API stands for Application Programming Interface. It consists of various communication protocols and subroutines that can be used by programs for inter-communication. There are various types of APIs available such as WEB APIs, LOCAL APIs, PROGRAM APIs, etcetera.

Types of API functions in Node.js:

<li>Asynchronous, Non-blocking functions</li>
<li>Synchronous, Blocking functions</li>

<br>

<b>Q7. What is JSON format? </b>

JavaScript Object Notation (JSON) is a standard text-based format for representing structured data based on JavaScript object syntax. It is commonly used for transmitting data in web applications (e.g., sending some data from the server to the client, so it can be displayed on a web page, or vice versa).


<b>Q8. Why we use JSON format for API?</b>

JSON is nothing more than the data structure part of the JavaScript programming language. That means by its very definition, it is a perfect fit to represent JavaScript objects.

But because most programming languages have similar models of how to represent structured data, JSON also is a good fit for the internal model of many other programming languages.

This meant that JSON was a much more natural fit for developers to exchange structured data. It did not require the rather inconvenient “data binding” and “data serialization” steps that were notoriously difficult when using XML-based APIs.

Instead, JSON allowed APIs to represent structured data in a way that simply was a better fit for the conceptual universe that most developers live in.

<b>Q9. What is a Framework?</b>

A framework is a set structure in which tasks are performed or completed.

Typically, a framework refers to an often layered structure that indicates what kind of programs can or should be built and how they would connect to each other.
Basically, a framework works as a kind of support structure for something to be built on top of.

A software framework is an abstraction in which software that provides generic functionality, can be selectively changed by additional user-written code, this provides application specific software.

Software frameworks are designed to be universal, and reusable to provide functionality as part of a larger software platform, this then facilitates the development of software applications, products, and solutions.

<b>Q10. How an HTTP Communication works.</b>

HTTP (Hypertext Transfer Protocol) is the set of rules for transferring files -- such as text, images, sound, video and other multimedia files -- over the web.

Through the HTTP protocol, resources are exchanged between client devices and servers over the internet. Client devices send requests to servers for the resources needed to load a web page; the servers send responses back to the client to fulfill the requests. Requests and responses share sub-documents -- such as data on images, text, text layouts, etc. -- which are pieced together by a client web browser to display the full web page file.

<b>Q11. What is Middleware in ExpressJS.</b>

Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. These functions are used to modify req and res objects for tasks like parsing request bodies, adding response headers, etc.

Middleware is commonly used to perform tasks like body parsing for URL-encoded or JSON requests, cookie parsing for basic cookie handling, or even building JavaScript modules on the fly.