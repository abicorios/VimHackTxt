# VimHackTxt
Info about my use vim
# _vimrc in Windows
The file
```
C:\Program Files\Vim\_vimrc
```
# utf8 in Windows
append to the _vimrc 
```
set encoding=utf-8
set fileencoding=utf-8
set guifont=Lucida_Console:h9:cANSI:qDRAFT
```
# how to understand Lucida_Console:h9:cANSI:qDRAFT
open the vim or the gvim
```
:set guifont=*
```
select the font in the menu, the Lucida_Console can show the utf8 simbols
```
set guifont?
```
now you see
```
guifont=Lucida_Console:h9:cANSI:qDRAFT
```
it is all about it

# Python, move all left on 4 space
in the vim
```
:%s/\(^.*\)/    \1/g
```
# Python, move lines 10-14 left on 4 space
in the vim
```
:10,14s/\(^.*\)/    \1/g
```
# how to enable the vi mode in the node repl
in the bash console
```
sudo apt update && sudo apt install rlwrap && echo 'alias node="env NODE_NO_READLINE=1 rlwrap node"'>>~/.bashrc && echo 'set editing-mode vi'>>~/.inputrc
```
# how to enable the vi mode and the tab completion in the irb
in the bash console
```
echo 'set editing-mode vi'>>~/.inputrc && echo "require 'irb/completion'">>~/.irbrc'
```
