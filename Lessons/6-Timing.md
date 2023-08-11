## Timing

You may have heard the phrase "Timing is everything" before. That phrase is very true when it comes to animation. Animation is all about time. You use seconds to your advantage, greatly changing the way a animation looks and feels. Timing will help sell the believabilty of your animation.

When animating we are constantly getting the viewer to "buy in", to get invested in the story and characters. We want them to forget that they are watching a series of still images. The timing of those still images enhances that buy in, that investment. It eases the suspension of disbelief.

So far we've used ease in, ease out, and linear values for animation/transition-timing-function. There are more options for those settings. We can get most customization using cubic-bezier curves.

>A cubic Bézier easing function is a type of easing function defined by four real numbers that specify the two control points, P1 and P2, of a cubic Bézier curve whose end points P0 and P3 are fixed at (0, 0) and (1, 1) respectively. The x coordinates of P1 and P2 are restricted to the range [0, 1].
-[w3](https://www.w3.org/TR/css-easing-1/#cubic-bezier-easing-functions)

You can achieve ease in, ease out, ease-in-out, etc by using cubic-bezier. This is admitted easier done if you are good at math, which I am not. I read some articles that I'll share here to help with understanding it:

[Advanced CSS Animation Using cubic-bezier()](https://css-tricks.com/advanced-css-animation-using-cubic-bezier/) by Temani Afif

[Cubic Bézier: from math to motion](https://blog.maximeheckel.com/posts/cubic-bezier-from-math-to-motion/) by Maxime Heckel

I personally learn better by doing. If you are like me, you'll want to play around with cubic-bezier to get a better understanding. You can do that visually with this [cubic-bezier generator](https://cubic-bezier.com).

I took the [staging animation](https://codepen.io/crystal-williams-brown/pen/bGQayrW) I made and changed the timing function.

original `animation-timing-function: ease-out;`

new `animation-timing-function: cubic-bezier(.32,.33,.7,.95);`

This allowed me freedom to remove some keyframes, since the cubic-bezier curve would handling the change in speed.

original
```
@keyframes arc {
  0%{
    transform: translate(0%, 8%) rotate(-6deg);
  }
  15%{
    transform: translate(50%, 0%) rotate(0deg);
  }
  35%{
    transform: translate(100%, 8%) rotate(6deg);
  }
  60%{
    transform: translate(80%, 12%) rotate(-8deg);
  }
  100%{
    transform: translate(40%, 25%) rotate(-15deg);
  }
   from {border-bottom: 100px solid  #fcf3cf;}
  to {border-bottom: 100px solid  #aed6f1;}
}
```
new
```
@keyframes arc {
  0%{
    transform: translate(0%, 8%) rotate(-6deg);
  }
  35%{
    transform: translate(100%, 8%) rotate(6deg);
  }
  100%{
    transform: translate(40%, 25%) rotate(-15deg);
  }
   from {border-bottom: 100px solid  #fcf3cf;}
  to {border-bottom: 100px solid  #aed6f1;}
}
```

Further work with the curve and keyframes can smooth this out even more. You can try this out with my [code pen for timing](https://codepen.io/crystal-williams-brown/pen/QWJXavr) or/and make your own.

***
## Assignment
Use the cubic-beizer to adjust the timiing of your animation.


#### Requirements:
You can either use my code pen or make your own, or do both. Modify the timing of the animation using cubic-beizer.

Here is the link to my Code Pen on timing https://codepen.io/crystal-williams-brown/pen/QWJXavr
