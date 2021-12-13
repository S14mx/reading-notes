# Day 2 assignment

## Using external CSS

### **`<link>`** Element

The `<link>` element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. It is an empty element (meaning it doesn't need a closing tag), and it lives inside the `<head>` element. It should use three attributes:

### **href**

This specifies the path to the CSS file (which is often placed in a folder called *css* or *styles*).

### **type**

This attribute specifies the type of document being linked to. The value should be *text/css*.

### **rel**

This specifies the relationship between the HTML page and the file it is linked to. The value should be *stylesheet* when linking to a CSS file.
An HTML can use more than one CSS style sheet. To do this it could have a `<link>` element for every CSS file it uses. For example, some authors use one CSS file to control the presentation (such as fonts and colors) and a second to control the layout.

HTML document:

```html
<!DOCTYPE html>
  <html>
    <head>
        <title>Using external CSS</title>
        <link href="css/styles.css" type="text/css" rel="stylesheet"/>
    </head>
    <body>
        <h1>Potatoes</h1>
        <p>Potatoes are good</p>
    </body>
  </html>
```

CSS document:

```css
body {
  font-family: arial;
  background-color: blue;}
h1 {
  color: red;}
```

### [_Go back to main page_](README.md)
