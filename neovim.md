### Cursor Moving
1. h <-, j (Down), k (Up), l ->

### Line Commands
1. x: (Delete the character under cursor)
2. i: (To start inserting the text)
3. A: (Appending text to the end of the line)
4. dw: (Delete all the characters till next space)
5. d$: (To delete to the end of line)
6. 0: (Cursor to the start of line)
7. nw: (Move the cursor n words forward)
8. ne: (Move the cursor n words to it's last character)
9. dnw: (Delete n words)
10. dd: (To delete the whole line) [The line is registered with Neovim]
11. ndd: (To delete n lines)
12. u: (To undo the last action)
13. U: (To undo the actions on line)
14. Ctrl + r: (To redo the command)
15. p: (To paste the line below the cursor)
16. P: (To paste the line above the cursor)
17. r, R: (Replace the current character)
18. ce: (Delete the word till end and Enter Insert mode)
19. c$: (Delete till end of line for change)
20. /: (To search for an expression) [n && N]
21. ?: (To search in reverse direction) {Ctrl + o}
22. %: (When on a parenthesis, to find its closing match)
23. :s/old/new (For substituting the text) [/g for global]
24. :%s/old/new/g (For changing in the whole file) [/gc for prompt]
25. :! (To execute an external command)
26. o, O: (For insert mode)
27. v: (Visual Mode), y: (Copy), p: (Paste)
28. <Space>: For everything to look out.

### Exiting Files
1. :q! (Exit without saving)
2. :wq (Write to file and exit)
3. Ctrl + g: (File info at the bottom)
4. G: To the bottom of the file.
5. gg: To the start of the file.
6. :w (To save the file) [:w <name>]
7. :r FILENAME (Copy contents and place below cursor)

### Some Concepts
1. :Tutor (For learning the fundamentals of Neovim)

