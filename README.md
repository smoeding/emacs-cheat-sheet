# Emacs Cheat Sheet

This is a collection of Emacs keybindings that I should use more often.

## Mark Ring

Key                    | Command
-----------------------|--------------------------------------------------
<kbd>C-SPC C-SPC</kbd> | Set the mark, pushing it onto the mark ring, without activating it.
<kbd>C-u C-SPC</kbd>   | Move point to where the mark was, and restore the mark from the ring of former marks.
<kbd>C-x C-SPC</kbd>   | Move point to buffer and position of the last entry in the global ring (`pop-global-mark`).

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

## Registers

Key                    | Command
-----------------------|-----------------------------------------------
<kbd>C-x r SPC R</kbd> | Record the position of point and the current buffer in register R (`point-to-register`)
<kbd>C-x r j R</kbd>   | Jump to the position and buffer saved in register R (`jump-to-register`)
<kbd>C-x r s R</kbd>   | Copy region into register R (`copy-to-register`)
<kbd>C-x r i R</kbd>   | Insert text from register R (`insert-register`)
<kbd>C-x r +</kbd>     | Append text to or increment register (`increment-register`)

## Abbrevs

Key                  | Command
---------------------|-----------------------------------------------
<kbd>C-x a g</kbd>   | Define an abbrev, using one or more words before point as its expansion (`add-global-abbrev`)
<kbd>C-x a l</kbd>   | Similar, but define an abbrev specific to the current major mode (`add-mode-abbrev`)
<kbd>C-x a i g</kbd> | Define a word in the buffer as an abbrev (`inverse-add-global-abbrev`)
<kbd>C-x a i l</kbd> | Define a word in the buffer as a mode-specific abbrev  (`inverse-add-mode-abbrev`)

## Calc

Key                | Command
-------------------|-----------------------------------------------
<kbd>C-x * g</kbd> | Open Calc and add region as vector (`calc-grab-region`)
<kbd>v p</kbd>     | Pack stack elements as vector; prefix is length (`calc-pack`)
<kbd>v u</kbd>     | Unpack vector on the top of the stack (`calc-unpack`)
<kbd>V S</kbd>     | Sort elements of a vector (`calc-sort`)
<kbd>I V S</kbd>   | Sort elements of a vector in decreasing order
<kbd>u #</kbd>     | Count number of values in a vector (`calc-vector-count`)
<kbd>u +</kbd>     | Sum values in a vector (`calc-vector-sum`)
<kbd>u *</kbd>     | Multiply values in a vector (`calc-vector-product`)
<kbd>u M</kbd>     | Compute mean of values in a vector (`calc-vector-mean`)
<kbd>H u M</kbd>   | Compute median of values in a vector (`calc-vector-median`)
<kbd>u S</kbd>     | Calculate sample standard deviation (`calc-vector-sdev`)
<kbd>I u S</kbd>   | Calculate population standard deviation (`calc-vector-pop-sdev`)
<kbd>t U</kbd>     | Convert between date and Unix time value (`calc-unix-time`)
