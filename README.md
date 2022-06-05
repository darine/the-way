Given a  pattern of 1,2,4,8 neing N,E,S,W then the bits represent connections in this arrangement:

WSEN

Then a clockwise rotation is:

1. left-shift <<
2. AND with the 5th bit (16)
3. If true, subtract 15 (-16, +1) to get the LSB turned on

And an anti-clockwise rotation is:

1. AND with 1st bit (1)
2. zero-fill right-shift >>>
3. If step 2 is true, add 8 to get the MSB turned on


