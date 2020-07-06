# HP50G
HP50G Goodies
I'm an Electrical Engineer, with a specialty in designing radio's.
There are a couple of dozen equations that I use fairly frequently, and
I've programmed them into PEQEM rather than use Excel because of the
numeric solver and multiple equation solver that's built into the 50G.

Asciiflow (http://www.asciiflow.com/ ) is a useful website/drawing tool
that will create ASCII drawing for documentation. While it's not as nice
looking at a GROB, it's a lot faster to put together, and text is all
that PEQEM supports.

Since I like typing on a large keyboard as well, I use a SD card to hold
text files, and translate them on the calculator from ASCII format to
directories and variables. I've also developed a couple of utility
programs to assist with this, and I'll document them here. I use
AsciiBin (http://www.hpcalc.org/details.php?id=3648) to go from a text
string on the stack to HP50g executable objects. I've renamed
ASCIIBIN.49 to UZ on my calculator, just to make things easier to type.

First, the PEQUM Equation Directory. This is a cut down version of the
one I use, as that one is ~ 20k of ASCII. I use the @ as a comment
delimiter, and try to format equations so that they are readable. This
text file resides in the root directory of the SD Card.

PEQUM is located here http://www.hpcalc.org/details.php?id=6306 , and is
a pretty handy equation library routine.

In practice, I recall this text file from the SD Card to the stack, and
then run UZ on it, to translate it to a directory. I can then "EVAL"
this, and the object on the stack will purge the old 'EQUATION'
directory and store the new one into the same one. Below is the program
that I use (from the home directory) to pull EQ02.txt and a Notes file.
The Notes File is a simple text file that I display using VV, which is
the text display part from ( http://www.hpcalc.org/details.php?id=7213).
When I update either text file on the SD card, I run this utility, which
I've named rclSD, to pull from the SD card and install on the
calculator.
