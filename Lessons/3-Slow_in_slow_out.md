## Slow In, Slow Out:

While some things move at a continuous speed there are many things that adjust speed due to resistance. We have wind, gravity or even the structure of our body that changes the speed of our actions. The timing adjusts, speeding up and slowing down. This adjustment feels natural and can help your animation be more appealing as well as realistic. Often consistent speed is associated with inorganic things such as machinery. It has it's place. But to create a friendly, human feel it is common to use timing changes even for machines.

For showing different timings we will use transition and transition-timing-function attributes. CSS has settings for the following transition-timing-function:
- linear, where the timing is consistent from start to end
- ease-in, where the transition starts slower than it ends
- ease-out, where the transition ends slower than it starts
- ease-it-out, where the transition starts and ends slower than the speed it has in the middle

There are other things you can do with timing, such as manually skipping frames. Like so `transition-timing-function: steps(2, jump-start);`. This has us skip 2 frames at the start of the transition. [More details on transitions can be found in Modzilla docs](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-timing-function)

***

## Assignment
You will be animating a shape moving and show the difference between ramping up it's speed (slow in) and ramping down it's speed (slow out)


#### Requirements:
Setup a code pen and make 2 versions of the shape. Have each one use a different timing (slow in, slow out).

Here is the link to my Code Pen where I animated different timings
https://codepen.io/crystal-williams-brown/pen/zYMwvoJ
