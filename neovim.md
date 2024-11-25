## **Cursor Movement (Basics)**
1. `h`: Move left
2. `l`: Move right
3. `j`: Move down
4. `k`: Move up
5. `w`: Move to the start of the next word
6. `e`: Move to the end of the current/next word
7. `b`: Move to the beginning of the previous word
8. `ge`: Move to the end of the previous word
9. `0`: Move to the start of the current line
10. `^`: Move to the first non-blank character of the line
11. `$`: Move to the end of the line
12. `G`: Move to the bottom of the file
13. `gg`: Move to the top of the file
14. `{`/`}`: Move to the start/end of the current paragraph
15. `Ctrl-d`: Scroll down half a page
16. `Ctrl-u`: Scroll up half a page
17. `Ctrl-f`: Scroll one page forward
18. `Ctrl-b`: Scroll one page backward

## **Editing and Text Manipulation**
1. `x`: Delete the character under the cursor
2. `i`: Insert mode before the cursor
3. `I`: Insert mode at the beginning of the line
4. `a`: Insert mode after the cursor
5. `A`: Insert mode at the end of the line
6. `o`: Open a new line below the current line
7. `O`: Open a new line above the current line
8. `r`: Replace the current character
9. `R`: Replace mode (overwrites text)
10. `dd`: Delete the current line
11. `ndd`: Delete `n` lines
12. `dw`: Delete to the start of the next word
13. `d$`: Delete to the end of the line
14. `ce`: Change (delete and switch to insert mode) until the end of the word
15. `c$`: Change until the end of the line
16. `yy`: Copy the current line
17. `nyy`: Copy `n` lines
18. `p`: Paste after the cursor
19. `P`: Paste before the cursor
20. `u`: Undo the last action
21. `Ctrl-r`: Redo the last undone action
22. `y{motion}`: Yank (copy) text based on motion commands (`yw`, `y$`, etc.)
23. `v` / `V` / `Ctrl-v`: Visual mode (character, line, and block selection)

## **Search and Replace**
1. `/pattern`: Search forward for `pattern`
2. `?pattern`: Search backward for `pattern`
3. `n`: Repeat the last search forward
4. `N`: Repeat the last search backward
5. `:%s/old/new/`: Replace `old` with `new` in the entire file
6. `:%s/old/new/g`: Replace all occurrences in the entire file
7. `:%s/old/new/gc`: Replace all with confirmation
8. `*`: Search for the word under the cursor forward
9. `#`: Search for the word under the cursor backward
10. `%`: Jump to the matching bracket/parenthesis

## **Window Management**
1. `:split`: Split window horizontally
2. `:vsplit`: Split window vertically
3. `Ctrl-w w`: Move between windows
4. `Ctrl-w h/j/k/l`: Move to left/down/up/right window
5. `Ctrl-w +`: Increase the height of the window
6. `Ctrl-w -`: Decrease the height of the window
7. `Ctrl-w =`: Equalize all window sizes
8. `Ctrl-w c`: Close the current window

## **Tab Management**
1. `:tabnew FILENAME`: Open a file in a new tab
2. `gt`: Move to the next tab
3. `gT`: Move to the previous tab
4. `:tabs`: List all tabs
5. `:tabclose`: Close the current tab

## **Buffers**
1. `:bnext` / `:bn`: Switch to the next buffer
2. `:bprev` / `:bp`: Switch to the previous buffer
3. `:bd`: Close the current buffer
4. `:ls`: List all buffers
5. `:buffer N`: Switch to buffer `N`

## **File Management**
1. `:w`: Save the current file
2. `:q`: Quit
3. `:wq`: Save and quit
4. `:q!`: Quit without saving
5. `:e FILENAME`: Open a file
6. `:r FILENAME`: Read the contents of a file and insert it at the cursor
7. `:w FILENAME`: Save to a specific file

## **Plugins and Advanced Features**
1. **Built-in LSP**:
 - `:LspInfo`: Show active LSP servers
 - `gd`: Go to definition 
 - `gD`: Go to declaration
 - `gr`: Go to references
 - `gi`: Go to implementation
 - `K`: Show hover documentation
 - `<leader>rn`: Rename symbol

2. **Tree-sitter** (Advanced Syntax Highlighting):
 - Install with `:TSInstall`
 - Use `:TSUpdate` to keep it up-to-date

3. **File Explorer (e.g., Nvim-Tree)**:
 - Open file explorer: `:NvimTreeToggle`
 - Navigate and open files easily

4. **Fuzzy Finder (e.g., Telescope)**:
 - `:Telescope find_files`: Search for files
 - `:Telescope live_grep`: Search for text in files
 - `:Telescope buffers`: List and switch buffers
 - `:Telescope help_tags`: Search through help documentation

5. **Git Integration** (via Fugitive or GitSigns):
 - `:Git`: Open Git commands interface
 - `[c`: Previous Git hunk
 - `]c`: Next Git hunk
 - `:Gwrite`: Stage changes
 - `:Gread`: Discard changes

6. **Formatting**:
 - `:lua vim.lsp.buf.format()`: Format the current buffer using LSP

## **Customization Tips**
1. **Keymaps**: Define custom shortcuts in your `init.lua` or `init.vim`.
2. **Themes**: Install and configure themes like Gruvbox or Dracula.
3. **Plugins**: Use a plugin manager (e.g., `packer.nvim` or `vim-plug`) to extend functionality.
4. **Autocommands**: Automate actions like saving files or enabling specific settings for certain file types.

## **Help and Learning**
1. `:Tutor`: Learn the fundamentals interactively
2. `:help [command]`: Get detailed help for a specific command
3. `:checkhealth`: Diagnose Neovim setup issues

