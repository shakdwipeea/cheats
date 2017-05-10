### Emacs reference
For setup using http://www.braveclojure.com/basic-emacs/

## files

1. In Emacs, editing takes place in buffers.
2. To switch to a buffer, use C-x b and enter the buffer name in the minibuffer.
3. To create a new buffer, use C-x b and enter a new buffer name.
4. To open a file, use C-x C-f and navigate to the file.
5. To save a buffer to a file, use C-x C-s.
6. To create a new file, use C-x C-f and enter the new file’s path. When you save the buffer, Emacs will create the file on the filesystem.

## movement

| Keys  | Description                                                                                    |
|-------|------------------------------------------------------------------------------------------------|
| C-a   | Move to beginning of line.                                                                     |
| M-m   | Move to first non-whitespace character on the line.                                            |
| C-e   | Move to end of line.                                                                           |
| C-f   | Move forward one character.                                                                    |
| C-b   | Move backward one character.                                                                   |
| M-f   | Move forward one word (I use this a lot).                                                      |
| M-b   | Move backward one word (I use this a lot, too).                                                |
| C-s   | Regex search for text in current buffer and move to it. Press C-s again to move to next match. |
| C-r   | Same as C-s, but search in reverse.                                                            |
| M-<   | Move to beginning of buffer.                                                                   |
| M->   | Move to end of buffer.                                                                         |
| M-g g | Go to line.                                                                                    |

## cut copy

| Keys | Description                            |
|------|----------------------------------------|
| C-w  | Kill region.                           |
| M-w  | Copy region to kill ring.              |
| C-y  | Yank.                                  |
| M-y  | Cycle through kill ring after yanking. |
| M-d  | Kill word.                             |
| C-k  | Kill line.                             |

## editing

| Keys | Description                                                                 |
|------|-----------------------------------------------------------------------------|
| Tab  | Indent line.                                                                |
| C-j  | New line and indent, equivalent to enter followed by tab.                   |
| M-/  | Hippie expand; cycles through possible expansions of the text before point. |
| M-\  | Delete all spaces and tabs around point. (I use this one a lot.)            |

## emacs window bindings

| Keys  | Description                                                                                                                                       |
|-------|---------------------------------------------------------------------------------------------------------------------------------------------------|
| C-x o | Switch cursor to another window. Try this now to switch between your Clojure file and the REPL.                                                   |
| C-x 1 | Delete all other windows, leaving only the current window in the frame. This doesn’t close your buffers, and it won’t cause you to lose any work. |
| C-x 2 | Split frame above and below.                                                                                                                      |
| C-x 3 | Split frame side by side.                                                                                                                         |
| C-x 0 | Delete current window.                                                                                                                            |

## clojure buffer key bindings

| Keys        | Description                                                                        |
|-------------|------------------------------------------------------------------------------------|
| C-c M-n     | Switch to namespace of current buffer.                                             |
| C-x C-e     | Evaluate expression immediately preceding point.                                   |
| C-c C-k     | Compile current buffer.                                                            |
| C-c C-d C-d | Display documentation for symbol under point.                                      |
| M-. and M-, | Navigate to source code for symbol under point and return to your original buffer. |
| C-c C-d C-a | Apropros search; find arbitrary text across function names and documentation.      |

## cider buffer key bindings

| Keys     | Description                     |
|----------|---------------------------------|
| C-↑, C-↓ | Cycle through REPL history.     |
| C-enter  | Close parentheses and evaluate. |

## paredit key bindings
| M-x paredit-mode | Toggle paredit mode.                                                     |
|------------------|--------------------------------------------------------------------------|
| M-(              | Surround expression after point in parentheses (paredit-wrap-round).     |
| C-→              | Slurp; move closing parenthesis to the right to include next expression. |
| C-←              | Barf; move closing parenthesis to the left to exclude last expression.   |
| C-M-f, C-M-b     | Move to the opening/closing parenthesis.                                 |
