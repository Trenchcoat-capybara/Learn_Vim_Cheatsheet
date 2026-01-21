# Vim cheatsheet

# modes

keybind     mode                    function
ctrl + c    go to command mode      command mode is where you move around and decide where to edit

## Vim motions
keys used in command mode to move the cursor.

Motion  Usage
gg      Go to the beginning of the buffer.
G       Go to the end of the buffer.
0       Go to the beginning of the line (it is a zero).
$       Go to the end of the line.
w       Go forward one word.
b       Go backward one word.
h       Go left.    h, j, k, l = right, down, up, left
j       Go down.
k       Go up
l       Go right
)       Go forward one sentence
(       Go backward one sentence.

you can use a number infront of motion to perform that motion several times at once
5j = jjjjj = go down five time

## Insertion starters

Motion  Usage
i       Insert at cursor.
I       Insert before the first non-whitespace character in the current line.
a       Append text after the cursor.
A       Append text at the end of the current line.
o       Open a new line below the position
O       Open a new line above the current line.

## Range opertaion

Operator    Usage
c           Change the range-that is, delete the characters and move into insert mode at the beginning of the range
d           Delete the range.
y           Yank the range-that is, copy it to a register (Vim's version of a clipboard) ready to paste later.
g~          Invert the range case (change uppercase characters to lowercase characters and vice versa).
gU          Make the range uppercase ("go upper").
gu          Make the range lowercase ("go lower").
!           Send the range through the external program
