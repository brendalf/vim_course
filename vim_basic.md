# Vim Basic

Let's the fun begin.

## Vim Modes

Vim has five modes:

**Normal**: Default mode, used most for navigation and code editing.
    `Esc` to enter.
    `[hjkl]` to navigate.
**Insert**: Used for writing in the document.
    `[iIaAoO]` to enter.
**Replace**: Used for rewriting in the document.
    `[rR]` to enter.
**Command**: Used for typing commands.
    `:` to enter.
**Visual**: Used most for selection, copying and cliping.
    `[vV] or Ctrl+v` to enter.

> You can combine vim commands with numbers.

## Navigating

While in the **Normal mode** you can execute:

`[hjkl]` to navigate.
`gg` to jump to the begging of the file.
`G` to jump to the end of the file.
`[{}]` to jump between code blocks.
`[wbe]` to navigate between words.
`f` to navigate to a caracter.
`0` to jump to the beggining of the line.
`^` to jump to the first char of the line.
`$` to jump to the end of the line.
`:X` jump to line X.

## Commands
You can write your onw config inside `~/.vimrc` file.
For neovim, the config is inside the `~/.config/nvim/init.vim` file.

Basic:
``````
:set number
:set relativenumber
:set hidden
:set cursorline
:h command
``````

Identation:
``````
:set shiftwidth=4
:set tabstop=4
``````

In vim we can have different configs for each filetype / programming language.
``:autocmd FileType yaml setlocal shiftwidth=2 tabstop=2``

Tabs:
``````
:tabedit
:tabprev
:tabnext
``````
Windows:
``````````
:split
:vsplit
To navigate: Ctrl+w hjkl
``````````

## Editing

**Normal mode**
`u` to undo.
`Ctrl+r` to redo.
`yy` to copy line.
`yw` to copy a word.
`y$` to copy to the end of the file.
`pP` to paste below.
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

**Command mode**
`:!` to execute programs in terminal.
`:r!` to execute programs in terminal saving the output in the document.

**Visual mode**
`[uU]` to lowercase/uppercase.
`d` to delete.
`y` to copy text.
`[<>]` to ident lines.

**Recording**
`q a` to record macro a.
`q` to stop recording.
`@a` to apply macro a.
`@@` to repeat last macro.
