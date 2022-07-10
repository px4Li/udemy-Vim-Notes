# Udemy Tutorial - Vim Masterclass

## Vim Essentials
- ### Navigation Commands

    - press ***"j"*** to move down a line
    - press ***"k"*** to move up a line
    - press ***"l"*** to move the right
    - press ***"h"*** to move the left
    - ***"Ctrl-f"*** is the same as the ***"Page Down"***
    - ***"Ctrl-b"*** is the same as the ***"Page Up"***
    - Use ***"w"*** to move forward by word.
    - Use ***"Shift-w"*** to move forward and ignore punctuation
    - Use ***"b"*** to move backward by word.
    - Use ***"Shift-b"*** to move backward and ignore punctuation
    - Use ***"0"*** or ***"Shift-^"*** to move to the first character in the line
    - Use ***"Shift-$"*** or ***":*** + ***\$"*** to move to the end character in the line
    - Use ***"number*** + ***gg"*** or ***"number*** + ***Shift-g"*** or ***":*** + ***number*** + ***press Enter"*** to go to specific line
    - Use ***"gg"*** to go to first line in the file
    - Use ***"Shift-g"*** to go to last line in the file
    - Turn on ***":*** + ***set ruler"*** to get cursor location
    - Turn off ***":*** + ***set noruler"*** to disable to show line infor
    - Or toggle turn on/off the ruler just use ***":*** + ***ruler!"***
    - Use ***"Ctrl-g"*** to show how many lines in the file and cursor location 
    - Use ***"g*** + ***Ctrl-g"*** to get more information about the current cursor location

- ### Deleting Text
    - Use ***"x"*** or ***"d*** + ***l"*** to delete a character at the cursor
    - Use ***"Shift-x"*** or ***"d*** + ***h"*** to delete a character left the cursor and the character at the cursor will not be deleted
    - ***"d*** + ***j"*** to delete current line you're on and the line below it
    - ***"d*** + ***k"*** to delete current line you're on and the line above it
    - Use ***"d*** + ***w"*** to delete a word 
    - Use ***"number*** + ***d*** + ***w"*** or ***"d*** + ***number*** + ***w"*** to delete how many words
    - Use ***"number*** + ***d*** + ***number*** + ***w"*** to delete how many words by how many times
    - Use ***"d*** + ***0"*** to delete all the way to the beginning of the line from your current cursor position
    - Use ***"d*** + ***$"*** or ***"Shift-d"**** to delete current cursor position all the way to the end of the line
    - Use ***"d*** + ***d"*** to delete the entire line
    - Use ***"number*** + ***d*** + ***d"*** to delete how many lines
    - Use ***"."*** to repeat the previous command