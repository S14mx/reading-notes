# Adding Images

`<img>`\
To add an image into the page you need to use an `<img>` element. This is an empty element (which means there is no closing tag). It must carry the following two attributes:

## *src*

This tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site. (Here you can see that the images are in a child folder called images — relative URLs were covered on pages 83-84).

## *alt*

This provides a text descriptionof the image which describes theimage if you cannot see it.

``` html
<img src="images/quokka.jpg" alt="A family of quokka" title="The quokka is an Australian marsupial that is similar in size to the domestic cat." />
 ```

## *title*

You can also use the title attribute with the `<img>` element to provide additional information
about the image. Most browsers will display the content of this attribute in a tootip when the
user hovers over the image. The text used in the alt attribute is often referred to as alt text.
It should give an accurate description of the image content so it can be understood by screen reader software (used by people with visual impairments) and search engines.If the image is just to make a page look more attractive (and it has no meaning, such as a graphic dividing line), then the alt attribute should still be used.

### *From HTML & CSS: Design and Build Websites by Jon Duckett; ISBN*978-1-118-00818-8

### [_Go back to main page_](README.md)