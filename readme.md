# Bonobos Homework Assignment

## Joe Bliss

## Instructions

Simply download the zip or clone this repo above. Open `index.html` in your browser and enjoy! A working version is viewable online at: http://josephjbliss.github.io/bonobos

## My Approach

I generally try to pre-program as much in the CSS with classes as I can, so that a lot of JS becomes `addClass()`, `toggleClass()`, `removeClass()`, and checking for hasClass(). This is the approach I took. I loaded the image at the 3x size and shrunk it to the height or width of the viewport (depending on the size / shape of the viewport) with CSS. Then, when the user clicked on zoom in, I removed that restriction. This allowed me to avoid using absolute or fixed positioning and complicated math and animation. So, having this image naturally overflowing allowed me to tie the scroll position (scrollLeft and scrollTop) of the #wrapper to the position of the mouse on mousedown and mousemove.

## What I Would Improve

It wound up being a litte trickier than I thought it would be at first. There is definitely refactoring that could happen, and I think I would take a more OO approach if I was starting again - defining a ZoomablePhoto that could be created / destroyed - than just directly manipulating the DOM. My approach wound up being a little more "spaghetti" than I'm totally proud of.
