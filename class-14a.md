# Class Reading 14a

## CSS Transforms
With CSS3 came new ways to position and alter elements. 

All of these new techniques are made possible by the transform property.

The transform property comes in two different settings, two-dimensional and three-dimensional.

Transform Syntax
The actual syntax for the transform property is quite simple, including the transform property followed by the value.

2D Transforms
Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane.

2D Rotate
The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees.

2D Scale
Using the scale value within the transform property allows you to change the appeared size of an element. 

2D Translate
The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document.

2D Skew
The last transform value in the group, skew, is used to distort elements on the horizontal axis, vertical axis, or both. The syntax is very similar to that of the scale and translate values.

Combining Transforms
It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time for example. In this event multiple transforms can be combined together. To combine transforms, list the transform values within the transform property one after the other without the use of commas.

Transform Origin
Perspective
    - Perspective Depth Value
    - Perspective Origin

3D Transforms

Backface Visibility
When working with three-dimensional transforms, elements will occasionally be transformed in a way that causes them to face away from the screen.

## CSS Transitions & Animations
Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.

Transitional Properties
background-color
background-position
border-color
border-width
border-spacing
bottom
clip
color
crop
font-size
font-weight
height
left
letter-spacing
line-height
margin
max-height
max-width
min-height
min-width
opacity
outline-color
outline-offset
outline-width
padding
right
text-indent
text-shadow
top
vertical-align
visibility
width
word-spacing
z-index

Transition Duration
Transition Timing
Transition Delay

Shorthand Transitions
Declaring every transition property individually can become quite intensive, especially with vendor prefixes. Fortunately there is a shorthand property, transition, capable of supporting all of these different properties and values. Using the transition value alone, you can set every transition value in the order of transition-property, transition-duration, transition-timing-function, and lastly transition-delay. Do not use commas with these values unless you are identifying numerous transitions.

Animations
Animation Keyframes
To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

Animation Name
Animation Duration, Timing Function, Delay

Customizing Animations
Animation Iteration, Direction, Play State, Fill Mode

## 8 simple CSS3 transitions that will wow your users
Fade In
Fade in effects are coded in two steps: first, you set the initial state; next, you set the change. (Make sure you set the class of your div to “fade” to see this working.)

Change color
Animating a change of color used to be unbelievably complex, with all kinds of math involved in calculating separate RGB values and then recombining them.

Grow & Shrink
To grow an element, you used to have to use its width and height, or its padding.

Rotate Elements
CSS transforms have a number of different uses, and one of the best is transforming the rotation of an element. 

Square to circle
A really popular effect at the moment is transitioning a square element into a round one, and vice versa.

3D Shadow
This effect is achieved by adding a box shadow, and then moving the element on the x axis using the transform and translate properties so that it appears to grow out of the screen.

Swing
Not all elements use the transition property. We can also create highly complex animations using @keyframes, animation and animation-iteration.

Inset border
The ghost button is a button with no background and a heavy border. We can of course add a border to an element simply, but that will change the element’s position. We could fix that problem using box sizing, but a far simpler solution is the transition in a border using an inset box shadow.

## 6 buttons animated
Codepen resource to play around with different button animations.

## CSS3 Animations: Keyframes
Codepen resource for making cool animations with Keyframes.

## 404
Another resource for animations via codepen.
