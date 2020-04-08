# My Tiny Bag Of Vim Tricks

## Basic Operations

**Open a file**:  `vim /some/file`

**Open a file within vim**: `:e /some/file`

**Save file**: `:w`

**Exit vim**: `:q`

**Save and exit vim**: `:wq`

**Force save/exit (when you don't have permission)**: `:w!`, `:q!`, `:wq!` (but, _why_ don't you have permission?)


## Navigation

**Go to top**: `gg`

**Go to bottom**: `[shift] + g`

**Go to beginning of line**: `[home]`

**Go to end of line**: `[end]`

**Scroll up and down quickly**: `[PgUp]`, `[PgDown]`, or just mousewheel back and forth


## Searching

**Go to place containing some given string (i.e. search)**: `/somegivenstring`, then, hit `n` to cycle through occurrence.

**Highlight all occurrences of some given string (i.e. search)**: `/somegivenstring`

**Get rid of search highlights**: `/alskjdflksjdf` (basically mash on keyboard for a string that probably won't exist in your file)

**Search and replace via regex**: `:%s/something/somethingelse/gci`

Note: "gci" means replace all occurrences, confirm with user for each case, and do so case insensitively, which is usually what you want


## Highlighting

**Highlight characters (i.e. visual mode)**:

* `v` to highlight current character, `[left]`, `[right]`, `[up]`, `[down]` to highlight more characters

**Highlight line (i.e. visual line mode)**:

* `[shift] + v` to highlight current line, `[up]` or `[down]` to highlight more lines

**Highlight block (i.e. visual block mode)**:

* `[ctrl] + v` to highlight current character, `[left]`, `[right]`, `[up]`, `[down]` to highlight more characters as if you're drawing a box


## Copy/Pasting

**Copy (or "yank")**: `y` after highlighting what you want to copy

**Cut (or "delete")**: `d` after highlighting what you want to cut

**Cut current line**: `dd`

**Paste**: `p` to paste after current position or current line (depending on what you've copied/cutted)


## Indents

**Indenting lines left or right**: `<` or `>` after highlighting the lines

**Indenting lines left or right by more than one indent level**: press a number before hitting the `<` or `>`.

**Indent to the left by some number of spaces**: block-highlight those spaces and cut/delete


## Making Edits

`[insert]` to go into insert mode and start typing

`[esc]` to get out of insert mode


## Multiple Windows In Same Vim Session

**Get a top and bottom split of windows**: `:split`

**Get a left and right split of windows**: `:vsplit`

**Jump between windows**: `<ctrl> + w`, then `[left]`, `[right]`, `[up]`, `[down]` in the direction you want to jump

In each window you can do regular vim things. You can copy/paste/yank/cut/etc... between windows. You can exit each individual window and it won't quit vim until you exit the last window.


## Miscellaneous

**Activate syntax highlighting**: `:setf <language>`
