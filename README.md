# DigitBoard
A free-to-use Java library for FRC teams using the REV Digit MXP Display (am-3223) with their roboRIO. Runs in its own thread.

Info on the functions:

getInstance returns the instance of the Digit Board.
getA and getB will simply return if the button is pushed.
getALatch and getBLatch will remain true until the data is read.
getAonRisingEdge and getBOnRisingEdge is true only when the value has gone from false to true (it will only be true when the button is released).
getPotentiometer returns the value of the dial, scaled to be between 0 and 1, going up by tenths. All the way counterclockwise is 0, all the way clockwise is 1.
writeDigits will write the first four characters of a given string onto the board.
