# What is WebGl and Why use Three.js

Three.js is a 3D JS lib that enables developers to create 3D experiencies for the web.

it works with WebGL, but you can make it work with SVG and CSS. It will be not as good as WebGL and you will get performances issues.

--

## What is WebGL

- JS API
- Renders triangles at a remarkable speed
- Result can be drawn in a <canvas>
- Compatible with most modern browsers
- Uses the Graphic Processing Unit (GPU) that because is fast (JapaScript is proceed in CPU)
- Can be use for 2D (Pixeljs) but we will focus on 3D

--

The CPU can do calculations really fast but only one bu one (this is not actually right, modern CPU has multiple core). The GPU is a little slower but can do thousands of parallel calculations.

To draw a 3D model, the idea is to draw many triangles at the right position and colorize them so that they look the way we want.

The GPU will position all those point at once accordding to many factors.

Once the points are placed, the GPU will draw each visible pixel of those triangules.

Again, those thousands of pixels will be calculated and drawn in parallel extremely fast.

_The instruction to place the points and draw the pixels are written is shaders._

We provide a bunch of information to those shaders like the points positions, model transdormations, the camera coordinates and things get positions and colorized the way we want.

This is why native WebGL is so hard. _Drawing a single triangule on the canvas would take at least 100 lines of code._

Native WebGL benefits from existing a low level - you are talking to the GPU - which enables optimizations and more control.

--

## Three.js to the rescue

https://github.com/mrdoob/three.js
https://threejs.org

- JS library, MIT license
- Right above WebGL
- Creator: _Ricardo Cabello_ (Mr.doob)

Three.js drastically simplify the process of all of this:

- You don't have to provide the shaders
- You don't have to provide each point

_We can still interact with the WebGL and we can create our own shader and provide our own information._

We will do such things when:

1. We want to optimize things
2. When we want to do things that Three.js can't do

--

If you want to follow updates and discover exceptional projects, I advise you to follow the Mr.doob and Three.js twitter accounts:

https://twitter.com/mrdoob

https://twitter.com/threejs

--

## What about other libraries?

Three.js is the most popular WebGL library for good reasons that we already covered. It's very stable, it provides many features, the documentation is remarkable, the community is working hard on updates, and it's still close enough to native WebGL.

That's why it's probably better to learn Three.js.

But there are many other libraries, and some of them are amazing as well. Be curious, try them out, and experience their strength for yourself. You might even learn things that will be useful for your Three.js projects.
