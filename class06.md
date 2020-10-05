## Class 06: JS Object literals

### Object Literals

- Objects group together a set of variables and functions to create a model of something you would recognize from the real world.
- Like variables and named functions, properties and methods have a name and a value. In an object, that name is called a `key`. An object cannot have two keys with the same name. This is because keys are used to access their corresponding values. 
- Creating an object: Literal notation.
The object is the curly braces and their contents. The object is stored in a variable called hotel, so you would refer to it as the hotel object. Seperate each key from its value using a colon. Seperate each property and method with a comma (but not after the last value).

 <!-- var hotel = {
     name: 'Quay",
     rooms: 40,
     booked: 25,
     checkAvailability: function() Preturn this.rooms - this.booked;
     }
     }
 } -->

- you can acces the properties or methods of an object using dot notation.
- you can also access properties using square brackets.

### Document Object Model (DOM)

- The DOM specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.
- DOM trees have four types of nodes: Text nodes, element nodes, attribute nodes and document nodes
- you can select element nodes bytheir id or class attributes, by tag name or using CSS elector syntax
- When a DOM query can return more than one node, it will always return a NodeList
- From an element node, you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques.
- an element node can contain multiple text nodes and child elements that are siblings of each other.
- Browsers offer tools for viewing the DOM tree.

[Back to Home](https://andrewliming.github.io/reading-notes/)