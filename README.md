# nvim
Neovim config as per [The Primeagen](https://github.com/ThePrimeagen) instructions. 

## Where
In MacOS place in: ` Users/<name>/.config/nvim `

## Original Instructions
Follow the video on [YouTube](https://www.youtube.com/watch?v=w7i4amO_zaE&list=PLm323Lc7iSW_wuxqmKx_xxNtJC_hJbQ7R&index=7&ab_channel=ThePrimeagen)


## Some (custom and not) NVIM shortcuts to keep in mind

### Telescope

- leader pf:  project find (telescope fuzzy finder)
- C-p:        project git fuzzy finder (telescope)
- leader ps:  file fuzzy finder by text (telescope)
 
### Harpoon

- leader a:     add page to harpoon
- C-e:          toggle quick menu
- C-h:          switch to file 1
- C-t:          switch to file 2
- C-n:          switch to file 3
- C-s:          switch to file 4 

### LSP

- gd          : jump to definition
- K           : show info on symbol under cursor
- leader vws  : workspace symbol ?!?
- leader vd   : diagnostic ?!?
- [d          : diagnostic goto next
- ]d          : diagnostic goto prev
- leader vca  : code action ?!?
- leader vrr  : references ?!?
- leader vrn  : rename ?!?
- C-h         : signature help ?!?
- leader vca  : *vim code actions*, eg import modules and constants
 
### Inside a menu
- C-p:      previous item
- C-n:      next item
- C-y:      accept choice
- C-space:  complete

###  NVIM remaps

#### N Mode
- C-o       : jump back to previous position (eg after a gg)
- f <symbol>: jump on top of next instance of <symbol>
- F <symbol>: jump on top of prev instance of <symbol>
- t <symbol>: jump before next instance of <symbol>
- T <symbol>: jump after prev instance of <symbol>
- J         : append next line to current line with a space inbetween (cursor stays in place)
- C-d       : move half a screen down keeping cursor central
- C-u       : move half a screen up keeping cursor central
- leader p  : delete element sending it to the void register (won't replace current element in the local clipboard)
- leader y  : yank into the system clipboard
- C-f       : tmux opens a new project (not working ?!?)
- leader s  : replace the word under the cursor and all its instances with new text
- leader x  : makes current file executable
- C-^       : jump back to prev file (can jump back and forth)

#### V Mode
- J         : shift down
- K         : shift up

#### In search mode
- n         : search next keeping cursor central
- N         : search prev keeping cursor central


### Tips and Tricks
- V%=       : select everything inbetween brackets and format it
- :%s       : do something for the entire file 
    - eg :%s/ : search entire file
    - eg :%s/\(.\)oldtext(/newtext) 
- VYp       : copy current line on next line
- ci"       : jump inside next quoted text, delete text and get ready to type
- ca"       : jump where quoted text is, delete text AND quotes, get ready to type
- ciw       : cut-out word deletes current word and get ready to type
- C-V 5j I <text in here> ESC: add same text in current and next5 lines

### Commands 
 
- TSPlaygroundToggle  : shows the AST of the code in the editor (treesitter/playground)
