# CREATE & ACCESS OBJECTS CONSTRUCTOR NOTATION

To get a better idea of why you might want to create multiple objects on the same page, here is an example that shows room availability in two hotels.  

First, a constructor function defines a template for the hotels. Next, two different instances of this type of hotel object are created. The first represents a hotel called Quay and the second a hotel called Park.  

Having created instances of these objects, you can then access their properties and methods using the same dot notation that you use with all other objects.  

In this example, data from both objects is accessed and written into the page. (The HTML for this example changes to accommodate the extra hotel.)  

For each hotel, a variable is created to hold the hotel name, followed by space, and the word rooms.  
The line after it adds to that variable with the number of available rooms in that hotel. (The+= operator is used to add content to an existing variable.)

``` JavaScript
function Hotel (name, rooms, booked) { 
this.name = name; 
this.rooms = rooms; 
this.booked = booked; 
this.checkAvailability = function() 
return this.rooms - this.booked; 
} ; 
var quayHotel = new Hotel('Quay', 40, 25); 
var parkHotel = new Hotel( ' Park', 120, 77);
 
var details!= quayHotel name + ' rooms : '; 
detailsl += quayHotel.checkAvailability(); 
var elHotell = docurnent.getElementByid('hotell'); 
elHotell.textContent =details!; 
var details2 = parkHotel.name+ ' rooms: '; 
detai ls2 += parkHotel.checkAvailability(); 
var e1Hotel2 = document.getEl ementByid('hotel2'); 
elHotel2.textContent = details2; 

```

### *From JavaScript & jQuery: Interactive Front-End Web Development by Jon Duckett; ISBN 978-1-118-53164-8*

### [_Go back to main page_](README.md)