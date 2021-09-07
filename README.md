# Dynamic-Web-Pages-With-JavaScript

## JavaScript

JavaScript (JS) is a programming language that allows you to implement complex things on web pages. For example, anytime a web page does complex things such as displaying timely content updates, interactive maps, animated 2D/3D graphics or scrolling video jukeboxes, as oppossed to just sitting there and displaying static information, chances are JavaScript has some involvement. JavaScript is well known as the scripting language for web pages. However, many non browser environments such as [Node.js](https://developer.mozilla.org/en-US/docs/Glossary/Node.js), [Apache CouchDB](https://couchdb.apache.org), and [Adobe Acrobat](https://opensource.adobe.com/dc-acrobat-sdk-docs/acrobatsdk/) also use it. The style of programming that JavaScript uses is a [prototype-based](https://developer.mozilla.org/en-US/docs/Glossary/Prototype-based_programming), multi-paradigmed, single-threaded, dynamic language, supporting object-oriented, imperative, and declarative. The standards for JavaScript are the [ECMAScript Language Specification](https://tc39.es/ecma262/)(ECMA-262) and the [ECMAScript Internationalization API specification](https://tc39.es/ecma402/) (ECMA-402). The JavaScript documentation throughout MDN is based on the lastest draft versions of ECMA-262 and ECMA-402. Keep in mind that JavaScript is not to be confused with Java programming language. They are both trademarked by the same company; however, the two programming languages have very different syntax, semantics and use.  

### Tutorials

The following guides and tutorials will help you learn how to program in JavaScript:

For complete beginners with no previous experience in JavaScript, the following resources will get you started

-[Learning Area JavaScript topic](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)

-[JavaScript first steps](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps) This resource will answer some key questions such as: What is JavaScript?, what does it look like?, and what can it do?, as well as discussing key JavaScript features.

[JavaScript building blocks](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks) continues the coverage of JavaScript key fundamental features, and focuses on commonly encountered types of code blocks.

[Introducing JavaScript objects](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects) The object oriented nature of JavaScript is important to understand if you want to go further with your knowledge of the language, and write more efficient code.

[Asynchronous JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous) Asynchronous JS is used to effectively handle potential blocking oerations such as fetching resources from a server. 

[Client-side web APIs](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs) 

### JavaScript guide

[JavaScript guide](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide) is a much more detailed guide to JS language, for those who have previous programming experience.

### Intermediate

[Understanding client-side JavaScript frameworks](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Client-side_JavaScript_frameworks) JavaScript frameworks are an essential part of modern front-end web development, providing developers with proven tools for building scalable, interactive web applications. 

[A re-introduction to JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript)

[JavaScript data structures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)

[Equality comparisons and sameness](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness) JS provides three different value comparison operations: strict equality using ===, loose equality using ===, and the [Object.is()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/is) method.

[Closures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures) 

### Advanced

[Inheritance and the prototype chain](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain) 

[Strict Mode](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Strict_mode) Strict mode defines that you can't use any variable before initializing it.

[JavaScript typed arrays](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Typed_arrays) This is a mechanism for accessing raw binary data.

[Memory Management](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Memory_Management) This is the memory life cycle and garbage collection in JS.

[Concurrency model and Event Loop](https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop) 

### Reference

[JavaScript Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference)

[Standard objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects)

[Expressions and operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators)

[Statements and declarations](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements)

[Functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions)

### Tools & Resources

Below are some helpful tools for writing and debugging your JS Code.

[Firefox Developer Tools](https://developer.mozilla.org/en-US/docs/Tools)

[JavaScript Shells](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Shells) This allows you to quickly test snippets of JS Code.

[Learn JavaScript](https://learnjavascript.online) Learn JS in an interactive environment, with short lessons and interactive tests, guided by automated assessment. 

[Together JS](https://togetherjs.com) Collaborators using JS can help each other online in real time.

[Stack Overflow](https://stackoverflow.com/questions/tagged/javascript)

[JSFiddle](https://jsfiddle.net) Edit JavaScript, CSS, HTML and get live results. Use external resources and collaborate with your team online. 

[Plunker](https://plnkr.co) Online community for creating, collaborating, on and sharing your web development ideas. You can also edit your JS, CSS, & HTML files, and get live results and file structure. 

[JSBin](https://jsbin.com/?html,output) An open source collaborative web development debugging tool.

[Codepen](https://codepen.io) Collaborative web development tool used as a live result playground.

[StackBlitz](https://stackblitz.com) An online playground and debugging tool, which can host and deploy full-stack applications using React, Angular, etc.

[RunJS](https://runjs.app) A desktop playground and scratchpad tool, which provides live results and access to both Node and Browser APIs.

## Input and Output in JS

< html>

< head>
  
  < title>Hello World</title>

< /head>

< body>
 
First name: <input id="first_name">
Last name: <input id="last_name">
<button id="say">Say hi!</button>
 
< hr>

< div id="result"></div>
 
< script>

function say_hi() {
    var fname = document.getElementById('first_name').value;
    var lname = document.getElementById('last_name').value;
 
    var html = 'Hello <b>' + fname + '</b> ' + lname;
 
    document.getElementById('result').innerHTML = html;
}
 
document.getElementById('say').addEventListener('click', say_hi);
</script>
 
< /body>

< /html>

In the above example, the JS code has a function called **say_hi**. It used the **getElementByld** to locate the DOM element representing the input element with the id **first_name.** The object returned has a method **value** that will return the text the user has typed in that field. This technique is used to retrieve the content of both **input** fields and assign their content to two variables: **fname** and **Iname.** Afterwards, these variables are used to create HTML snippet and assign it to a new variable called **html.** Then the **innerHTML** attribute is set as *earlier* to show the HTML that is generated.

## JavaScript Variables

There are three ways to declare a JavaScript variable:


-Using var

-Using let

-Using const

This chapter uses var.

Variables are containers for storing data (values). In the following example, x, y, and z, are variables, declared with the var keyword:

var x = 5;

var y = 6;

var z = x + y;

So, in this example, you can expect that:

-x stores the value of 5

-y stores the value of 6

-z stores the value of 11

In the next example, we have price1, price2, and total, as variables

var price1 = 5;

var price2 = 6;

var total = price1 + price2;

As previously mentioned, since variables store date (values) the total = price1 + price2, which would be 11. 

### JavaScript Identifiers

All JavaScript variables must identified with unique names. These unique names are called identifiers. Identifiers can be short names, like x and z or more descriptive names, such as age, sum, and totalVolume. There are general rules for constructing names for variables (unique identifiers):

-Names can contain letter, underscores, digits, and dollar signs.

-Names must begin with a letter

-Names can also begin with $ and _

-Names are case sensative (so y and Y are different variables)

-Reserved words (like JS keywords) can't be used as names.

### The Assignment Operator

In JavaScript the equal sign (=) is an assignment operator not an equal to operator. For example, x = x + 5 can be assigned to x; therefore the value of x would be incremented by 5. In the event you wish to write the equal to operator in JS language, you would write it as (==).

### Declaring (Creating) JavaScript Variables

Creating a variable in JavaScript is called declaring a variable. You declare a JavaScript variable with the var keyboard:

var carName;

After the declaration, the variable has no value (or has the variable of undefined in JS). So, in order to assign a value to the variable, use the equal sign.

carName = "Volvo";   

or you can also assign a value to the variable when you declare it

var carName = "Volvo";

In the next example, a variable called carName was created and the value of "Volvo" was assigned to it. Then the value was "output" inside an HTML paragraph with id = "demo"

<p id="demo"></p>

<script>

  var carName = "Volvo";

  document.getElementById("demo").innerHTML = carName; 

</script>

### Value = undefined

In computer programs, variables are often declared without a value. In JavaScript variables declared without a value will have the value of undefined. In the example below, the variable carName will have the value of undefined after the execution of this statement. 

var carName;

However, in JavaScript you can **Re-Declare** a variable, and it will not lose its value. In the example below, the variable carName will still have the value "Volvo" after the execution of these statements:

var carName = "Volvo";

var carName;

### JavaScript Dollar Sign $

It's important to keep in mind that JavaScript identifiers (names) must begin with:

-A letter (a-z)

-A dollar sign ($)

-Or an underscore (_)

Since JavaScript treats a dollar sign as a letter, identifiers containing $ are valid variable names:

var $$$ = "Hello World";

var $ = 2;

var $myMoney = 5;

Use of the $ is not very common in JavaScript; however, in the JavaScript library jQuery, the main function $ is used to select HTML elements. In jQuery $("p") means select all p elements.

### JavaScript Underscore (_)

Since underscores in JavaScript are treated as letters, the identifiers that contain one are valid variable names. For example,

var _lastName = "Johnson";

var _x = 2;

var _100 = 5;

