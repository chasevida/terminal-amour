#VIM Basics
My VIM favourite short keys.

Short Keys | Operation
---------- | -------------
⇧          | Shift
⌘          | Command
⌥          | Option/Alt
^          | Control

#iTerm2 Tabs/Pane
Short Keys       | Operation
---------------- | -------------
⌘⇧D              | Create pane vertically
⌘D               | Create pane horizontally
⌥⌘ →             | Switch pane right
⌥⌘ ←             | Switch pane left

#vimrc
Short Keys       | Operation
---------------- | -------------
:edit ~/.vimrc   | Enter insert mode

#General
Short Keys | Operation
---------- | -------------
:i         | Enter insert mode
esc        | Exit insert mode into command mode
:w         | :write <filename> to write/save the file
:wq        | :write :quit write/save and quit
:q         | :quit

#Moving
Make sure you are in command mode.

Short Keys | Operation
---------- | -------------
j          | down (it has a decedent in it’s type)
k          | up (it has an ascendent in it’s type)
h          | left
l          | right
w          | goes forwards from word to word
b          | goes backwards from word to word
⇧W         | goes forwards whole words plus ,.
⇧B         | goes backwards whole words plus ,.
$          | move to the end of the line
^          | move to the beginning of the line
0          | move to the line beginning
gg         | move to the very beginning of a file
⇧G         | move the very end of a file
{{         | shift paragraph up
}}         | shift paragraph down
:14        | will go to line 14

You can only move if there is somewhere to move to. i.e. you can’t go right if there is no right character to move to.

#Find

Short Keys     | Operation
----------     | -------------
/\<phrase\>      | Search for a general string
f \<letter\>     | Forward search
F \<letter\>     | Backward search
t, \<letter\>    | Forward search - puts cursor directly in front of key
T, \<letter\>    | Backward search - puts cursor directly in front of key
[n] f \<letter\> | `8fg` Searches for the 8th occurrence of the letter g


#Repeater
Typing a number before a command will repeat the command of the total number input.

Short Keys | Operation
---------- | -------------
3j         | Will go down three lines
5k         | Will go up five lines.
4fN        | Will find the fourth occurrence forward of the letter N
egg        | Will go three lines before the beginning of the file.
3GG        | Will go three lines before the end of the file.
:14        | Will go to line 14


#Editing


Short Keys | Operation
---------- | -------------
x          | Delete forward
db         | Delete entire word before cursor
dw         | Delete entire word after cursor
2dw        | Delete 2 (or n) words before cursor
dd         | Delete the entire line
dj         | Delete the entire line
2dd        | Delete 2 (or n) lines
cw         | Remove word (cursor should be at beggining) and enter insert mode
2cw        | Remove 2 words (or n) and enter insert mode
cc         | Delete the entire line and enter insert mode
2cc        | Delete 2 (or n) lines and enter insert mode
ct"        | Will delete everything up to next double quote and enter insert mode
ct*        | ct[*] then any character will delete everything up to that character then enter insert mode
ci"        | Change Inside double quotes. Deletes everything between double quotes and enters insert mode
ci{ ci(    | Will delete everything inside these and enter insert mode
ca"        | Change around " will delete everything including the " and enter insert mode
u          | Undo


#Cut, Copy & Paste


Short Keys | Operation
---------- | -------------
d          | Will cut a word
y          | Yank or Copy
yw         | Copy word
yj         | Copy line
p          | Will paste after the cursor
10p        | Will paste it n times
P          | Will paste before the cursor
x          | Will cut under the cursor
12x        | Will cut n characters from under the cursor
X          | Will cut the character behind the cursor
4X         | Will cut n characters behind the cursor
