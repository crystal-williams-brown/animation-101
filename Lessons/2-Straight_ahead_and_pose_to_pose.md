## Straight Ahead and Pose to Pose:

In animation you use still frames ordered in a way to convey a sense of motion. How you create those frames changes the way that motion feels/looks.

Straight ahead animation is when you create the frames in order from beginning to end. This is usually reserved for more subtle animation or fluid animation. It's especially useful for animating motion that is slow. However this style can be tricky to do well and requires a good consistency of drawing so that you don't get unwanted mutation in the subject by the time you get to the end. This method works well for rotoscoping, where you are animating recorded motion from a living being. It can allow you to get more details into the motion of the animation and make it feel close to life.

Pose to pose animation is where you animate what are called "key frames" first then fill in the "in-betweens". This is the most common way to animate and the easiest to learn how to do. The key frames are the big moments of change in the animation. If you were animating the throwing of a ball the key frames would likely be the swing back to prepare for the throw, the top of the arc when the throwing begins, and the finish of the arc when the ball leaves the hand. You would draw this first, then go back and fill in the frames between. How many frames you use will change the look of the motion. We will cover this in a future lesson. Pose to pose is best for exaggerated motion, not fully realistic but still identifiable.

To make things simple we will visualize the different animation styles by changing the color of a shape. The start and the end color are the same. We start with red and end with yellow. How we get there is what changes the effect.

There are [keyframes in CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/@keyframes) that can be used to have more control over animating elements.
Keyframes let you control the intermediate steps by specifying what should happen at certain times. For color we will use percentages to adjust the background-color attribute. For straight ahead you can let the color naturally progress from red to yellow:
```
@keyframes straight-ahead {
  from {background-color: #e03131;}
  to {background-color: #ffc726;}
}
 ```
For pose to pose you can assert color stops you would like during the transition:
```
@keyframes pose-to-pose {
  0%   {background-color: #e03131;}
  25%  {background-color: #6931e0;}
  50%  {background-color: #2e52e4;}
  100% {background-color: #ffc726;}
}
```

***

## Assignment
You will be animating a shape changing color using the 2 different styles of animating frames, straight ahead and pose to pose.


#### Requirements:
Setup a code pen and make 2 versions of the shape and have each one use one of the forms of animating frames.

Here is the link to my Code Pen where I animated using the 2 forms https://codepen.io/crystal-williams-brown/pen/LYgrmQv

#### Bonus Practice:
Add a play button to play the animations
