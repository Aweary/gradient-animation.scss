Summary
=======================

Sass mixin that lets anyone easily implement an animated background gradient. Currently this mixin requires Bourbon
but this is not a permanent dependency.


Usage
=======================

After you've included the SCSS file into your project you simply need to include it in the stylesheet for the element
you'd like to animate, like so

_@include animation-gradient($direction, $duration, ($colors...));_


The mixin takes three arguments:

__$direction:__ This is the direction of the linear animation, e.g., 125deg.

__$duration:__ The total animation time in seconds, e.g., 40s. I recommend 30s+ for a smooth gradient.

__$colors:__ This is a list of colors you'd like to include in the animation. Pass the list inside parantheses. There is no hard set limit to the number of colors that can be set, but I'd recommend keeping it between 2 and 6. 

Example
========================

element {
  @include gradient-animation(125deg, 50s, (#ff44ff, #aaff33, #33dd33, #33ff55));
}

outputs:
