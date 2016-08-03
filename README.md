# Flipdot Matrix Utils

Simple Python scripts to scroll text or display a GIF animation on a flipdot display from Alfazeta, using RS485 serial protocol.

## Background
I bought a flipdot display from Alfazeta at [flipdots.com](http://www.flipdots.com/) since I am fascinated by merging old-school technology with modern data. 

I wanted to control the display from a Raspberry Pi, but the example code I got was Arduino. I converted some of the code and wrote new functions to handle text-to-binary and GIF-to-binary instructions. 

## The two scripts

**textdot.py** will let you scroll a text of arbitrary length on the flipdot display. It's using a 5x7 bitmap font which is hard to read, but works. 

** imagedot.py** expects a GIF file, which can be animated. The image should be exactly the same size as the matrix, 28x14, and the script loops through the frames and animates the flipdots. The GIF I used in the example is not black-and-white, but the script assumes that any color besides white is "black", except when shown on the flipdot colors are inverted... I might change that. :)

