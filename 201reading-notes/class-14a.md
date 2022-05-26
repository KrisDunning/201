[Return to Course 201 Notes](https://KrisDunning.github.io/201/)

# Reading 14a - CSS Transforms, Transitions and Animations

*****

### 2D CSS Transforms

Transform Syntax  

> transform: scale(1.5);

Transform : rotate(0deg) - rotate an element from 0 to 360 degrees. Positive value will rotate clockwise, Neg. value, counterclockwise.  

Transform : scale(2.0) - allows you to change the appeared size of an element. Default scale is 1.0. Use scaleX or scaleY for horizontal or vertical independent scaling.  

Transform : translate(10px,20px) - Works like relative positioning. Pushing an element in a direction without interrupting the normal flow of the document. Like scale, can translateX/Y for independent translation.  

Transform : skew (10deg) - Distorts elements on the horizontal axis, vertical or both.  

To use multiple transform properties together, list them without commas after a transform call.  

> transform: rotate(25deg) scale (.5) translate (10px, 20px);  

Transform-origin : 20px,50px - changes the origin point of a transform from default, dead center of an element. The first input is horizontal axis and the second is vertical.  

### 3D CSS Transforms

Transform: rotateX/Y/X(45deg) - rotate allows you to rotate over a specific axis. Once again Pos. values are clockwise and Neg. values are counterclockwise.  

Transform : scale(1.5) - scales on the z axis. Works best with other 3D elements in place or a rotate and perspective change.  

Transform : translateZ(50px) - A neg. value pushes element further away on z axis and pos. value pulls closer.  

Transform-style : preserve-3d - When a 3D transform is applied on an element nested within a parent which is also being transformed this must be put on the parent element above any nested transforms. This allows the children to appear in their own 3D plane while the **flat** value forces the transformed childen elements to lie flat on the 2D plane.  

Backface-visibility: hidden - When you face an element away from the screen, such as rotatY(180deg), you can choose whether to see the back of the element or not. Set hidden for not or visible to see.  

## Transitions & Animations

CSS3 transitions have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as hovered, focused, active or targeted.  

CSS3 animations allow the appearance and behavior of an element to be altered in multiple keyframes. Animations can set multiple points of transition upon different keyframes.  

Transitions must have a change in stat and different styles must be identified for each state. The easiest way determining styles for different states is by using the :hover, :focus, :active, :target pseudo-classes.  

There are four transition related properties in total :  

- transition-property
- transition-duration
- transition-timing
- transition-delay

Not all are required to build a transition.  

**Not all properties may be transitioned**. They must have an identifiable halfway point. Here is a list of some transitional properties.

- background-color
- background-position
- border-color
- border-width
- border-spacing
- bottom
- clip
- color
- crop
- font-size
- font-weight
- height
- left
- letter-spacing
- line-height
- margin
- max-height
- max-width
- min-height
- min-width
- opacity
- outline-color
- outline-offset
- outline-width
- padding
- right
- text-indent
- text-shadow
- top
- vertical-align
- visibility
- width
- word-spacing
- z-index

Transition-duration - how long it takes for the transition to complete. Can be set with normal timing values (2s, 30ms, .5s). We can set multiple durations, one for each property. The order ***does*** matter. First transition-duration will match up to first transition-property. If only one duration value is included it will apply to all transition-properties. 

Transition-timing-function - sets the speed in which a transition will move. There are some popular keywords which can be used such as linear, ease-in, ease-out, ease-in-out.  
linear moves at a constant speed from one state to another.  
ease-in starts slowly and speeds up throughout the transition.  
ease-out starts quickly and slows down throughout the transition.  
ease-in-out starts and ends slow but speeds up in the middle.  

Transition-delay - sets a normal time value (sec, millisec) that determines how long a transition should be stalled before executing. Like others you can declare multiple values comma seperated.  

## Animations

Transitions handle single state changes but when more control is required or when transitions require multiple states then Animations are the answer.  

### Animation Keyframes

@keyframes - is used to declare the multiple points the element should make a transition. The @keyframes rule should include the animation name, any animation breakpoints and the properties intended to be animated.  

~~~~~CSS
@keyframes slide {
  0% {
    left: 0;
    top: 0;
  }
  50% {
    left: 244px;
    top: 100px;
  }
  100% {
    left: 488px;
    top: 0;
  }
}
~~~~~

The animatinos keyframe is names 'slide' and its keyframe breakpoints are listed as '%'s' of duration of transition. Remember that animations can only apply to a single property, not from one to another. So no (top:0 to bottom:0. It needs to be top:0 to top:100).  

Animation-name : slide - Once the animation keyframes are declared they need to be assigned to an element. To do that we use the animation-name property.  

### Animation Duration, Timing Function and Delay

Once we have declared the name, animations behave similarly to transitions. 

Animation-duration : 2s - We can set the duration in normal time sec/ms.  

Animation-timing-function: - Works the same as the transition property.  

Animation-delay : .5s - Works the same as the transition property.  

### Customizing Animations

Animations can be customized such as declare how many times an animation runs and which direction in which the animation completes.  

Animation-iteration-count: infinite - provide a integer or infinite keyword to set number of times to repeat the animation.  

Animation-direction: normal - Values for this property are normal, reverse, alternate and alternate-reverse. Reverse plays an animation from the 100% keyframe backwards. Alternate will play animation forward then backwards. Each journey 0-100% and 100%-0 each count as an iteration, so take that into account. Alternate also inverts ease-in and ease-out timing-functions. Alternate-reverse combines both and doubles the confusion....  

Animation-play-state: paused - allows an animation to be played or paused using the running and paused keywords. 

Animation-fill-mode: none - identifies how an element should be style either before, after, or before and after an animation is run. The fill mode accepts 4 values.  

- none - not apply any styles to an element before or after animation has run
- forwards- keep styles declared within the last specified keyframe. These styles may be changed based on the animation direction and iteration count. 
- backwards - will apply the styles in the first specified keyframe.
- both - apply the behaviors from both the forwards and backwards values


## Things I wish I knew more about

how do transitions apply to canvas objects? i wonder how that could work together. 

*****

[Return to Course 201 Notes](https://KrisDunning.github.io/201/)