# SIMPLE CSS3 TRANSITIONS

## Fade in

Fade in effects are coded in two steps: first, you set the initial state; next, you set the change, for example on hover:

``` css
.fade
{
        opacity:0.5;
}
.fade:hover
{
        opacity:1;
}

```

## Change color

Animating a change of color used to be unbelievably complex, with all kinds of math involved in calculating separate RGB values and then recombining them. Now, we just set the div’s class to “color” and specify the color we want in our CSS:

``` css
.color:hover
{
        background:#53a7ea;
}
```

## Grow & Shrink

To grow an element, you used to have to use its width and height, or its padding. But now we can use CSS3’s transform to enlarge.

``` css
.grow:hover
{
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
}
```

Shrinking an element is as simple as growing it. To enlarge an element we specify a value greater than 1, to shrink it, we specify a value less than 1:

``` css
.shrink:hover
{
        -webkit-transform: scale(0.8);
        -ms-transform: scale(0.8);
        transform: scale(0.8);
}
```

## 3D shadow

This effect is achieved by adding a box shadow, and then moving the element on the x axis using the transform and translate properties so that it appears to grow out of the screen.

``` css
.threed:hover
{
        box-shadow:
                1px 1px #53a7ea,
                2px 2px #53a7ea,
                3px 3px #53a7ea;
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
}
```

### From [www.webdesignerdepot.com](https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users)

### [_Go back to main page_](README.md)