# BREAKPOINTS

You can pause the execution of a script on any 
line using breakpoints. Then you can check the 
values stored in variables at that point in time. 

## DEBUGGER KEYWORD

You can create a breakpoint in your code using just the 
debugger keyword. When the developer tools are open, this 
will automatically create a breakpoint.  

You can also place the debugger keyword within a conditional 
statement so that it only triggers the breakpoint if the condition is 
met. This is demonstrated in the code below.  

It is particularly important to remember to remove these statements before your code goes live as this could stop the page running if a user has developer tools open.  

``` JavaScript

var $form, width, height, area; 
$form = $('#calculator') ; 
$('#calculator').on('submit', function(e) 
e.preventDefault(); 
console.log('Clicked submit. . . '); 
width = $('#width').val(); 
height = $('#height').val(); 
area = (width* height); 
if (area < 100) { 
debugger; // A breakpoint is set i f the devel oper tools are open 
}
$form.append('<p> ' + area + '<I p>'); 
} ) ;

```

![result pic](https://raw.githubusercontent.com/S14mx/reading-notes/main/pics/screenclass10.png)

### *From JavaScript & jQuery: Interactive Front-End Web Development by Jon Duckett; ISBN 978-1-118-53164-8*

### [_Go back to main page_](README.md)