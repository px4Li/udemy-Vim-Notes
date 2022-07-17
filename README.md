<p style="text-align: center;"> Udemy Tutorial - Vim Masterclass (Jason Cannon)</p>

## 1. Vim Essentials
### 1.1. Navigation Commands

- press ***j*** to move down a line
- press ***k*** to move up a line
- press ***l*** to move the right
- press ***h*** to move the left
- ***Ctrl-f*** is the same as the ***Page Down***
- ***Ctrl-b*** is the same as the ***Page Up***
- Use ***w*** to move forward by word.
- Use ***Shift-w*** to move forward and ignore punctuation
- Use ***b*** to move backward by word.
- Use ***Shift-b*** to move backward and ignore punctuation
- Use ***0*** or ***Shift-^*** to move to the first character in the line
- Use ***Shift-$*** or ***:*** + ***\$*** to move to the end character in the line
- Use ***number*** + ***gg*** or ***number*** + ***Shift-g*** or ***:*** + ***number*** + ***press Enter*** to go to specific line
- Use ***gg*** to go to first line in the file
- Use ***Shift-g*** to go to last line in the file
- Turn on ***:*** + ***set ruler*** to get cursor location
- Turn off ***:*** + ***set noruler*** to disable to show line infor
- Or toggle turn on/off the ruler just use ***:*** + ***ruler!***
- Use ***Ctrl-g*** to show how many lines in the file and cursor location 
- Use ***g*** + ***Ctrl-g*** to get more information about the current cursor location

### 1.2. Deleting or Text
- Use ***x*** or ***d*** + ***l*** to delete a character at the cursor
- Use ***Shift-x*** or ***d*** + ***h*** to delete a character left the cursor and the character at the cursor will not be deleted
- ***d*** + ***j*** to delete current line you're on and the line below it
- ***d*** + ***k*** to delete current line you're on and the line above it
- Use ***d*** + ***w*** to delete a word 
- Use ***number*** + ***d*** + ***w*** or ***d*** + ***number*** + ***w*** to delete how many words
- Use ***number*** + ***d*** + ***number*** + ***w*** to delete how many words by how many times
- Use ***d*** + ***0*** to delete all the way to the beginning of the line from your current cursor position
- Use ***d*** + ***$*** or ***Shift-d**** to delete current cursor position all the way to the end of the line
- Use ***d*** + ***d*** to delete the entire line
- Use ***number*** + ***d*** + ***d*** to delete how many lines
- Use ***.*** to repeat the previous command

## 2. Deleting=Cut, Yanking=Copy & Putting=Paste
- ***d*** and ***x*** cut text, not just delete it.
- cut = delete and save into a register.
- Register is a clipboard-like storage locattion.
- Use ***p*** to place a text on the line below where the cursor is.
- Use ***shift-p*** to place a text on the line up where the cursor is.
- Use ***number*** + ***y*** + ***w*** or ***y*** + ***number*** + ***w*** to copy spesifed the numbers word.
- Use ***number*** + ***yy*** to duplicate spesified the numbers line.
- Use ***u*** to undo it
- Use ***Ctrl-r*** to redo it
- Unnamed register = ""
- Numbered registers = 0 1 ... 9
-  holds text from d, c, s, x, and y operations.
- 0 holds last text yanked (y).
- 1 holds last text deleted (d) or changed (c).
- Numbered registers shift with each d or c.
- Use ***:reg*** to look at the registers
- Use black hole register ***"_*** will not register in Registers
- Use 26 named registers from a to z (Captial A to B will append to a to b), like ***"a*** to specify a register, then copy it by useing ***yy***
- Use the register, you can use ***"a*** + ***p*** to paste the line you registered or in multiple case ***number*** + ***p***
- Use ***:reg*** space ***a*** to look at a specific register or in multiple case add mutiple named and numbered registers

## 3. Transforming and Substituting Text
### 3.1. Inserting, Changing, Replacing, and Jointing
- Use ***shift-i*** to jump to the first non blank character in the line and switch to insert mode.
- Use ***i*** to switch to insert mode but the cursor will not jump.
- Use ***a*** to append text after the current cursor position. 
- Use ***shift-a*** to jump to end of the line and place you in insert mode.
- Use ***o*** to begin a new line below the cursor and place you in insert mode.
- Use ***shift-o*** to create a line above the current line and start inserting mode
- Use ***number*** + ***i*** + ***symbols/charctors*** + ***Esc*** to create a line that contains numbers of symbols/charactors
- Use ***number*** + ***o*** + ***symbols/charctors*** + ***Esc*** to create numbers line that contains numbers of symbols/charactors
- Use ***shif-r*** to place you to replace mode
- Use ***r*** + ***symbol/charactor*** to replace the current cursor charactor. Note it just can replace one charactor.
- Use ***c*** + ***w*** to change/delete a word where is the cursor on that word of the beginning. Then you will into insert mode.
- Use ***c*** + ***$*** or ***shift-c*** to replace from your current cursor position all the way through the end of the line.
- Use ***cc*** to replace entire line of text
- Use ***~*** to change lowercase to uppercase vice versa
- Use ***g*** + ***~*** + ***w*** to change the case of a word
- Use ***g*** + ***~*** + ***$*** or ***0*** to change the case from current cursor position to the end of the line or beginning of the line
- Use ***g*** + ***~~*** to change the case of the entire line no matter the cursor where is it.
- Use ***g*** + ***u*** or ***shift-u*** + ***w*** to change the case of the word to lowercase or uppercase no matter what case they were before.
- Use ***g*** + ***uu*** or ***shift-u shift-u*** to change the case of the entire line no matter what case they were before.
- Use ***shift-j*** to combine two lines on one line. But between the two sentences will have two space.
- Use ***numbers*** + ***shift-j*** to combine all numbers of lines to join together.
- Use ***g*** + ***shift-j*** to combine two lines and will not have space between two sentences.