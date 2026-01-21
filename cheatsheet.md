# Vim cheatsheet

## modes

keybind     mode                    function
ctrl + c    go to command mode      command mode is where you move around and decide where to edit.\n

## Vim motions
keys used in command mode to move the cursor.\n

Motion  Usage\n
gg      Go to the beginning of the buffer.\n
G       Go to the end of the buffer.\n
0       Go to the beginning of the line (it is a zero).\n
$       Go to the end of the line.\n
w       Go forward one word.\n
b       Go backward one word.\n
h       Go left.    h, j, k, l = right, down, up, left\n
j       Go down.\n
k       Go up.\n
l       Go right.\n
)       Go forward one sentence.\n
(       Go backward one sentence.\n

you can use a number infront of motion to perform that motion several times at once.\n
5j = jjjjj = go down five time.\n

## Insertion starters

Motion  Usage\n
i       Insert at cursor.\n
I       Insert before the first non-whitespace character in the current line.\n
a       Append text after the cursor.\n
A       Append text at the end of the current line.\n
o       Open a new line below the position\n
O       Open a new line above the current line.\n

## Range opertaion

Operator    Usage\n
c           Change the range-that is, delete the characters and move into insert mode at the beginning of the range.\n
d           Delete the range.\n
y           Yank the range-that is, copy it to a register (Vim's version of a clipboard) ready to paste later.\n
g~          Invert the range case (change uppercase characters to lowercase characters and vice versa).\n
gU          Make the range uppercase ("go upper").\n
gu          Make the range lowercase ("go lower").\n
!           Send the range through the external program\n

### examples
c2w     remove the next two words.\n

