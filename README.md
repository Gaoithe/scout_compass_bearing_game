# scout_compass_bearing_game
Calculate bearings and generate: post labels, bearing following instructions and game cheat sheet instructions.  

## Scout compass bearing challenge game

Posts are set out in a circle a good distance apart. 
One post starting at magnetic North,
 other posts at each compass point N NNE NE ENE E ESE . . . e.t.c.
Each post is labeled with name and has a scrambled alphabet in a grid.

Scouts receive an instruction sheet with start post and series of bearings to follow.
At each post visited a letter of a word is obtained. 

A simple grid reference for each post describes how to obtain a letter.
The grid reference at N post comes from the Irish grid reference system.
The letters in the grid are scrambled at each other post. 
https://en.wikipedia.org/wiki/Irish_grid_reference_system#/media/File:Irish_Grid.svg

A full scrambled alphabet is on each post. 
This allows a large combination of word instructions to be used.
It allows interesting quotes or song lyrics to be used as a challenge for a group of scouts.

e.g. of post label with post name and scrambled alphabet in grid:

```
########################################
#
# POST: 337.5 => NNW
#
#        1   2   3   4   5 - Easting
#
#    5   Y   H   T   M   G   
#    4   W   B   C   I   U   Q   
#    3   K   P   Z   R   L   
#    2   S   X   O   N   J   
#    1   F   V   E   D   A   
#     \
#      Northing
#
########################################
```

e.g. of instruction sheet for a two letter word:

```
########################################
#
# Word 0
# START at POST: 67.5 => ENE
#
# 0. Follow bearing 123.75 to next Post,
#    Record letter @ Easting 1, Northing 1  _______
# 0. Follow bearing 146.25 to next Post,
#    Record letter @ Easting 6, Northing 4  _______
#
########################################
```

e.g. of portion of cheat sheet

```
########################################
# Cheat Sheet
#
# Word 0 is We, post path is [67.5, 45.0, 22.5]
#    DEBUG post:45.0 c:W
#    DEBUG post:22.5 c:e
#
.
.
.
```

A python script is used . . . 
16 posts are currently used.
8 posts or other number can wasily be used with script adjustment.
The word list or quote used can be changed in script.
TODO: map and allow arbitrary positioning of posts e.g. in rectangle or other shape would be suitable for a permanently marked compass bearing challenge. 

The script is quite messy currently . . WIP . . beware of roadworks and dragons. 

## FILES:

The script, run:
`python scout_bearing_to_compasspoint.py`
Numpy is used a little bit, matplotlib is called but not needed to generate game instructions,

Output of script text post labels and word instructions:
scout_bearing_to_compasspointDEBUG.txt

Put the script in an open-office doc, insert a section around the post labels and in format->section make it two columns. Do the same around word instructions. Adjust labels/instructions so they do not wrap around a column or page. print. Cut up. Attach labels to posts. Have fun! 
scout_compass_bearing_posts.odt
scout_compass_bearing_posts.pdf


