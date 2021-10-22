# USING EVENT LISTENERS

In this example, the event listener appears on the last line of the JavaScript. Before you write an event listener, two
things are put in place:

1. If you use a named function when the event fires on your chosen DOM node, write that function first. (You could also use an anonymous function.)

2. The DOM element node(s) is stored in a variable. Here the text
input (whose id attribute has a value of username) is placed into
a variable called el Username.

``` JavaScript

function checkUsername() {                         // Declare function 
var elMsg = document.getElementByld('feedback');  // Get feedback element 
if (this.value.length < 5) {                     // If username too short  
elMsg.textContent = 'Username must be 5 characters or more'; // Set msg
} else {                                              // Otherwise 
elMsg.textContent = '';                            // Clear msg 
  }
}

var elUsername = document.getElementByld('username') ; // Get username input 
// When it loses focus call checkUsername() 
elUsername.addEventlistener('blur', checkUsername, false) ; 

```

### The addEventListener ()

method takes three properties: i) The event you want it to listen
for. In this case, the blur event. ii) The code that you want it
to run when the event fires. In this example, it is the checkUsername() function. Note that the parentheses are omitted
where the function is called because they would indicate that
the function should run as the page loads (rather than when the
event fires). iii) A Boolean indicating how events flow, see p260. (This is usually set to false.).

### BROWSER SUPPORT

Internet Explorer 8 and earfier versions of IE do not support the
addEventlistener() method, but they do support a method called attachEvent() and you will see how to use this on p258. Also, as with the previous example, IE8 and older versions of IE would not know what this referred to in the conditional statement. An alternative approach for dealing with it is shown on p270.

### EVENT NAMES

Unlike the HTML and traditional DOM event handlers, when you
specify the name of the event that you want to react to, the
event name is not preceded by the word "on". If you need to remove an event listener, there is a function called removeEventL i stener() which removes the event listener from the specified element (it has the same parameters).

### *From JavaScript & jQuery: Interactive Front-End Web Development by Jon Duckett; ISBN 978-1-118-53164-8*

### [_Go back to main page_](README.md)