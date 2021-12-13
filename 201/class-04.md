# Links

Links are created using the `<a>` element. Users can click on anything
between the opening `<a>` tag and the closing `</a>` tag. You specify
which page you want to link to using the href attribute.

``` html
<a href="http://www.imdb.com">IMDB</a>
```
## Linking to other sites

`<a>`\
Links are created using the `<a>` element which has an attribute called href. The value of the href attribute is the page that you want people to go to when they click on the link.Users can click on anything that appears between the opening `<a>` tag and the closing `</a>`tag and will be taken to the page specified in the href attribute.When you link to a different website, the value of the href
attribute will be the full web address for the site, which is known as an absolute URL.\
*Browsers show links in blue with an underline by default*

```html
<p>Movie Reviews:
<ul>
 <li><a href="http://www.empireonline.com">
 Empire</a></li>
 <li><a href="http://www.metacritic.com">
 Metacritic</a></li>
 <li><a href="http://www.rottentomatoes.com">
 Rotten Tomatoes</a></li>
 <li><a href="http://www.variety.com">
 Variety</a></li>
</ul>
</p>
```

## Linking to other pages on the same site

`<a>`\
When you are linking to other pages within the same site, you do not need to specify the domain name in the URL. You can use a shorthand known as a relative URL.If all the pages of the site are in the same folder, then the value of the href attribute is just the name of the file.If you have different pages of a site in different folders, then you can use a slightly more complex syntax to indicate where the page is in relation to the current page. You will learn more about these on the pages 81-84.If you look at the download code for each chapter, you will see that the index.html file contains links that use relative URLs

```html
<p>
<ul>
 <li><a href="index.html">Home</a></li>
 <li><a href="about-us.html">About</a></li>
 <li><a href="movies.html">Movies</a></li>
 <li><a href="contact.html">Contact</a></li>
</ul>
</p>
```

### *From HTML & CSS: Design and Build Websites by Jon Duckett; ISBN 978-1-118-00818-8*

### [_Go back to main page_](README.md)