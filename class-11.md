# Image Rollovers & Sprites

Using CSS, it is possible to create a link or button that changes to a 
second style when a user moves their mouse over it (known as a 
rollover) and a third style when they click on it. 

This is achieved by setting a background image for the link or button that has three different styles of the same button (but only allows enough space to show one of them at a time). You can see the image we are using in this example on the right. It actually features two buttons on the one image.  

When the user moves their mouse over the element, or clicks on it, the position of the background image is moved to show the relevant image.  

When a single image is used for several different parts of an 
interface, it is known as a sprite. You can add the logo and other 
interface elements, as well as buttons to the image.  

The advantage of using sprites is that the web browser only needs 
to request one image rather than many images, which can make the web page load faster.  

``` HTML

<a class="button" id="add-to-basket">
Add to basket</a>
<a class="button" id="framing-options">
Framing options</a>

```

``` CSS

a.button {
height: 36px;
background-image: url("images/button-sprite.jpg");
text-indent: -9999px;
display: inline-block;}
a#add-to-basket {
width: 174px;
background-position: 0px 0px;}
a#framing-options {
width: 210px;
background-position: -175px 0px;}
a#add-to-basket:hover {
background-position: 0px -40px;}
a#framing-options:hover {
background-position: -175px -40px;}
a#add-to-basket:active {
background-position: 0px -80px;}
a#framing-options:active {
background-position: -175px -80px;}

```






### *From HTML & CSS: Design and Build Websites by Jon Duckett; ISBN*978-1-118-00818-8

### [_Go back to main page_](README.md)