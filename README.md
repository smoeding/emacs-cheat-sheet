# Emacs Cheat Sheet

This is a collection of Emacs keybindings that I should use more often.

## Moving by Defuns

Key              | Command
-----------------|--------------------------------------------------
<kbd>C-M-a</kbd> | Move to beginning of current or preceding defun (`beginning-of-defun`)
<kbd>C-M-e</kbd> | Move to end of current or following defun (`end-of-defun`)
<kbd>C-M-h</kbd> | Put region around whole current or following defun (`mark-defun`)

## Editing with Parentheses

Key              | Command
-----------------|--------------------------------------------------
<kbd>C-M-f</kbd> | Move forward over a balanced expression (`forward-sexp`)
<kbd>C-M-b</kbd> | Move backward over a balanced expression (`backward-sexp`)
<kbd>C-M-k</kbd> | Kill balanced expression forward (`kill-sexp`)
<kbd>C-M-t</kbd> | Transpose expressions (`transpose-sexps`)
<kbd>C-M-n</kbd> | Move forward over a parenthetical group (`forward-list`)
<kbd>C-M-p</kbd> | Move backward over a parenthetical group (`backward-list`)
<kbd>C-M-u</kbd> | Move up in parenthesis structure (`backward-up-list`)
<kbd>C-M-d</kbd> | Move down in parenthesis structure (`down-list`)

## Abbrevs

Key                  | Command
---------------------|-----------------------------------------------
<kbd>C-x a g</kbd>   | Define an abbrev, using one or more words before point as its expansion (`add-global-abbrev`)
<kbd>C-x a l</kbd>   | Similar, but define an abbrev specific to the current major mode (`add-mode-abbrev`)
<kbd>C-x a i g</kbd> | Define a word in the buffer as an abbrev (`inverse-add-global-abbrev`)
<kbd>C-x a i l</kbd> | Define a word in the buffer as a mode-specific abbrev  (`inverse-add-mode-abbrev`)
