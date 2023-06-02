## Purpose:

The purpose of the 12 principles of animation is to lead to consistent quality animation. It aids in conveying motion in a believable way and builds a foundational understanding of physics. Thus allowing reliable creation of pleasing animations.

These principles can be applied to different types of animation including web animation.

## Goals:

Our goal is to have created 13 animations, the first 12 of which will highlight a different principle and the last will display all principles of animation.

## Tools:

We will be making web animations for this class using CSS. You will do your assignments in [Code Pen](https://codepen.io/) and show them to the class.

***

## Assignment

#### Context:
Consistency is a vital part of animation. Because of this we will focus on creating consistent shapes for our first assignment. This is very important for hand drawn animation, storyboards, character design, and layout sketches.

The key to consistent shapes is using your full arm rather than your wrist to draw, and practicing. Using a larger muscle group will help steady your motion and reduce fatigue. Be sure not to hold your writing implement too tightly, it’s better to use a loose/gentle grip.

Creating shapes in web animation requires different skills. You don't need to know how to draw but practicing drawing shapes consitently will help you with storyboarding animations. For web animation we use borders and size to make simple shapes. We'll use spans or divs to make our shapes.

To make a square you'll want the width and height to be the same size. You should add a background color so you can see the shape.

Here is the code the the square I made
```
.square {
  height: 100px;
  width: 100px;
  background-color: #2e52e4;
  display: inline-block;
}
```
Note: `display: inline-block;` is just to get the shapes to abide by sizing rules.

To make a circle is simple. The span/div has a `border-radius` property. To name a rounded edge square you could do

```
.square {
  height: 100px;
  width: 100px;
  background-color: #2e52e4;
  display: inline-block;
  border-radius: 8%;
}
```
By default `border-radius` is 0%. The greater the `border-radius` the rounder the shape. It maxes out at 100%. See if you can figure out how to make a circle.

Triangles are a bit harder. They rely on border properties. You'll want to set the width and height to 0 and allow the size to be determined by the border.

To set the width of the triangle, set the right and left borders to half of the width you want. So if you want your triangle to be `100px` wide, you'd set the left and right borders to `50px`. You'll want the borders to be solid (they can be dashes) and transparent since you will set the color using a different property.

To set the height of the triangle you use the `border-bottom` property. This is also where you set the color.

Here is a code I used to make a triangle
```
.triangle {
  width: 0;
  height: 0;
  border-right: 50px solid transparent;
  border-left: 50px solid transparent;
  border-top: 0;
  border-bottom: 100px solid #ffc726;
  display: inline-block;
}
```

Now that you know some general rules of making these basic shapes feel free to have fun with them. Customize them if you want.

#### Requirements:
Setup a code pen and make a circle, square and triangle. You can use these shapes for your future animation assignments. Feel free to make them your own.

Here is the link to my Code Pen where I made the shapes https://codepen.io/crystal-williams-brown/pen/vYVrRbv

#### Bonus Practice:
For each of the following shapes fill a single letter sized sheet of paper with rows of consistent drawings of it. The repetitions of the same shape should be visibly close to the same size and overall look.
  - Circle
  - Square
  - Triangle
