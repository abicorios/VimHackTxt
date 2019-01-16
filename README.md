# VimHackTxt
Info about my use vim
# _vimrc in Windows
```
C:\Program Files\Vim\_vimrc
```
# utf8 in Windows
append to _vimrc 
```
set encoding=utf-8
set fileencoding=utf-8
set guifont=Lucida_Console:h9:cANSI:qDRAFT
```
# how to understand Lucida_Console:h9:cANSI:qDRAFT
open vim or gvim
```
:set guifont=*
```
select font, Lucida_Console can show utf8
```
set guifont?
```
now you see
```
guifont=Lucida_Console:h9:cANSI:qDRAFT
```
it is all about it

# Python, move all left on 4 space
```
:%s/\(^.*\)/    \1/g
```
# Python, move lines 10-14 left on 4 space
```
:10,14s/\(^.*\)/    \1/g
```
# how to enable the vi mode in the node repl
```
sudo apt update && sudo apt install rlwrap && echo 'alias node="env NODE_NO_READLINE=1 rlwrap node"'>>~/.bashrc && echo 'set editing-mode vi'>>~/.inputrc
```
