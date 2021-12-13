# Floating Elements

### float

The float property allows you to take an element in normal flow and place it as far to the left or right of the containing 
element as possible.  
Anything else that sits inside the containing element will flow around the element that is floated.  
When you use the float property, you should also use the width property to indicate how wide the floated element should be. If you do not, results can be inconsistent but the box is likely to take up the full width of the containing element (just like it would in normal flow).  
In this example, a `<blockquote>` element is used to hold a quotation. It's containing element is the `<body>` element.  
The `<blockquote>` element is floated to the right, and the
paragraphs that follow the quote flow around the floated element.

``` html
<body>
<h1>The Evolution of the Bicycle</h1>
<p>In 1817 Baron von Drais invented a walking 
 machine that would help him get around...</p>
</body>
```

``` css
body {
width: 750px;
font-family: Arial, Verdana, sans-serif;
color: #665544;}
p {
width: 230px;
float: left;
margin: 5px;
padding: 5px;
background-color: #efefef;}
```
![result pic](https://raw.githubusercontent.com/S14mx/reading-notes/main/pics/book%20screen2.png)
### *From HTML & CSS: Design and Build Websites by Jon Duckett; ISBN*978-1-118-00818-8

### [_Go back to main page_](README.md)