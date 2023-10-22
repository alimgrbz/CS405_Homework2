# CS405_Homework2: Fragment Shaders
this is the second homework for Computer Graphics course
# CS 405 Homework 2 Report

## Introduction

This Homework is about changing an existing fragment shader to change the colour of an object from red to blue.

## Given Code

The given code was:


const fragmentShaderSource = `
precision mediump float;

void main() {
  gl_FragColor = vec4(1.0, 0.0, 0.0, 1.0);
}
`;

### Explanation

The first line determines the precision for the floats. There is a main function, and inside of it there is the line that is setting the color for the main fragment. `gl_FragColor` is a built-in variable that represents the final color of the current fragment. `vec4` is a 4-component vector. The four values provided represent the red, green, blue, and alpha (transparency) channels of the color, respectively. The values range from 0.0 to 1.0, where 1.0 is the maximum intensity/value for that channel.

### Modified Code

So the code that will set the color as blue is:
const fragmentShaderSource = `
precision mediump float;

void main() {
  gl_FragColor = vec4(0.0, 0.0, 1.0, 1.0); 
}
`;
