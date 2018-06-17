
// Use scale to change the scale of an element
/* Example: 
img {
  transform: scale(2);
}
*/

//will scale it to 2

// Use the skew function to skew the selected element along its X (horizontal) axis by a given degree.
/* Example: 

element1 {
  transform: skewX(25deg);
}

// Alternatevely the rotate function does the same thing as skewX and skewY
/* Example:

element1 {
  tranform: rotate(45deg);
}

// Use keyframes and animation properties when you want an animation that transitions.
// Transitions take s (seconds) and ms (miliseconds)
/* Example:

#rect {
  animation-name: rainbow;
  animation-duration: 4s;
} 

@keyframes {
  0% {
    background-color: blue;
  }
  
  50% {
    background-color: green;
  }
  
  100% {
    background-color: yellow;
  }
}

*/

// The animation-fill-mode specifies the style applied to an element when the animation has finished
/* Example:

  #rect {
    animation-name: background-color;
    animation-duration: 300ms;
    animation-fill-mode: forwards;
  }
*/

// Use the animation-iteration-count property to repeat an animation
// The animation-iteration-count property can take infinite as a value
/* Example: 

  #ball {
    animation-name: bounce;
    animation-duration: 1s;
    animation-iteration-count: infinite;
  }
  
*/

// To change the timing of the animation use the animation-timing-function property
// The animation-timing-function property takes ease (default), ease-in, ease-out and linear
/* Example: 

  #ball1 {
    animation-timing-function: linear;
  }

*/
