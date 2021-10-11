## Vim Basic
### Vim Config and Commands
You can write your onw config inside `~/.vimrc` file.
For neovim, the config is inside the `~/.config/nvim/init.vim` file.

Basic:
:set number
:set relativenumber
:set hidden
:set cursorline
:h command

Identation:
:set shiftwidth=4
:set tabstop=4

In vim we can have different configs for each filetype / programming language.
:autocmd FileType yaml setlocal shiftwidth=2 tabstop=2

Tabs:
:tabedit
:tabprev
:tabnext

Windows:
:split
:vsplit
To navigate: Ctrl+w hjkl

### Editing
**Normal mode**
`hjkl` to navigate.
    * You can add numbers.
`gg` to jump to the begging of the file.
`G` to jump to the end of the file.
`{}` to jump between code blocks.
`wbe` to navigate between words.
`f` to navigate to a caracter.
`$` to jump to the end of the line.
`u` to undo.
`Ctrl+r` to redo.
`:X` jump to line X.
`yy` to copy line.
`yw` to copy a word.
`y$` to copy to the end of the file.
`pP` to paste below.
`iIaA` to insert/append.
`oO` to add new line.
`cc` to substitute the whole line.
`ciw` to change word.
`x` to delete char by char.
`dd` to delete whole line.
`cw` to change to the end of the word.
`c$` to change to the end of the line.
`.` repeat last command.
`J` to join with line below.
`gJ` to join with line below (without space).

**Insert mode**

**Replace mode**
`r` to replace one character.
`R` to enter replace mode.

**Command mode**
`:!` to execute programs in terminal.

**Visual mode**
`uU` to lowercase/uppercase.
`d` to delete.
`y` to copy text.
`<>` to ident lines.

**Recording**
`q a` to record macro a.
`q` to stop recording.
`@a` to apply macro a.
`@@` to repeat last macro.
