## General cheat sheet
* Terminal: Ctrl-A/Ctrl-E for Home/End
* vimperator: zZ ==> reset zoom

## Tmux cheat sheet
* ```<Prefix> &``` for killing a window
* ```<Prefix> x``` for killing a pane
* ```<Prefix>(hold) [j|k|l|h]``` for resizing pane

## Vim cheat sheet

* . ==> repeat last change in normal mode
* same command on contiguous lines
	1. Select the lines you want to modify using Ctrl-v.
	2. Press:
	    * I: Insert before what's selected.
	    * A: Append after what's selected.
	    * c: Replace what's selected.
	3. Type the new text.
	4. Press Esc to apply the changes to all selected lines.

* You can use it with the d command, to delete all lines that contain a particular pattern, or all lines that do not contain a pattern. 
	* For example, to delete all lines containing "profile" (remove the /d to show the lines that the command will delete):
	<br>**$ :g/profile/d**
	* More complex patterns can be used, such as deleting all lines that are empty or that contain only whitespace:
	<br>**$ :g/^\s*$/d**


* The command to repeat an f is ; (semicolon) <br> , (comma) reverses the direction of the search.

* Use the normal command in Ex mode to execute the macro on multiple/all lines:

	Execute the macro stored in register a on lines 5 through 10.<br>
	**:5,10norm! @a**

	Execute the macro stored in register a on lines 5 through the end of the file.<br>
	**:5,$norm! @a**

	Execute the macro stored in register a on all lines.<br>
	**:%norm! @a**
	
	Execute the macro store in register a on all lines matching pattern.<br>
	**:g/pattern/norm! @a**

* vim copy visual mode seletected text to system clipboard 

	https://askubuntu.com/questions/613170/vim-and-system-clipboard
	
	"+y to yank, Ctrl-Shift-v to paste
* **:set list** to disply invisible characters

## Bug list
### js 
* with 'use strict' keyword, omitting declaration can lead to undesirable behaviors
* remember to refresh page with ctrl-shift R to clear page cache!
* When using children.length, be careful that even removed elements may affect it!
