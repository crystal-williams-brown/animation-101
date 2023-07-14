## Arc:

We see arcs in the way jointed limps move, the way trees sway in wind, in the rise and set of the sun, etc. Arc is the result of having an anchor at one point and and opposite point being able to move within the restrictions of that anchor and being fairly ridged so as not to fold.

For this principle we will anchor our object, the anchor can be anything. I decided my anchor was a head on which my object was placed. The arc is constrained by being worn as a hat. It is following the arc of the head/neck which is constrained by its connection to the torso.

In CSS we can use the animation and transformation attribute. You can set the translate and rotate to effect the arc. Often a object rotates a bit during it's arc.

To create the arc you can transform the shape using translate, which positions the shape within the screen. We will combine translation with the keyframes we used for the [straight ahead and pose to pose lesson](2-Straight_ahead_and_pose_to_pose.md).

Below is an example where percentages are used in the keyframes.

```
.triangle {
  position: absolute;
  width: 0;
  height: 0;
  border: 45px solid transparent;
  border-top: 0;
  border-bottom: 100px solid #ffc726;
  animation: arc 4s forwards;
  animation-timing-function: ease-out;
}

@keyframes arc {
  0%{
    transform: translate(0%, 8%) rotate(-6deg);
  }
   100%{
    transform: translate(50%, 0%) rotate(0deg);
  }
}
```
The first percentage is the amount of the animation time that the individual transformation with utilize. It's starting with 0% because this is before the animation begins. You can add more percentages with different transformations and each one will be a keyframe.
```
@keyframes arc {
  0%{
```
The percentages for the translation are determining how far the movement goes based on the parent of the object. You don't have to use percentages, you can get more exact. The first percentage controls the left to right, the second controls the up and down.
`transform: translate(0%, 8%)`

The rotate option lets you add a tilt/rotation to your object that will be either clockwise or counterclockwise depending on if the number is positive or negative.
`rotate(-6deg);`

animation timing-function is like the transistion-timing-fuction from our [slow in slow out lesson](3-Slow_in_slow_out.md).
`animation-timing-function: ease-out;`
***

## Assignment
You will be animating a shape moving in an arc. The way the arc plays out will depend on the object and its anchor. Pick the anchor, object and animate the arc accordingly.


#### Requirements:
Setup a code pen and animate a shape moving in an arc.

Here is the link to my Code Pen where I animated an arc
https://codepen.io/crystal-williams-brown/pen/abQEryM
