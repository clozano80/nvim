# nvim
Personal nvim configuration:
With coc, prettier, nerdcomment,...

##installation
- Install nvim (apt?)
- create .config/nvim
- upload files
- alias vim="nvim"


Inside nvim/vim
:checkhealth "comprobamos que funciona
:PlugInstall 
:CocInstall

:CocCommand #example snippets
:CocInstall coc-snippets

##special key
<space>

#Help Api autocomplete
<ctrl>+P
:gd (go to definition)
F2 rename all files with...

## move between splits or windows
<ctrl+w> <H,J,K,L>
<ctrl+w>W "next window
<ctrl+w>q  "quit
<ctrl+w>v/h split v or horizontal
<ctrl+w> <number optional> ">/</+/-"   decrease or increase split window

## nredtree
ctrl+n
select file and "t" #Open in tab 
select file and "i" split Horz
select file and "v" split Vertical

##Comment
Visual mode select and <space>cc
++ Comenter toggle in visual

## terminal
<space>t

## next tab
ctrl+t

##Prettier
:Prettier or <ctrl+i>

##Search FZF
:Ag [PATTERN]	ag search result (ALT-A to select all, ALT-D to deselect all)
:Rg [PATTERN]	rg search result (ALT-A to select all, ALT-D to deselect all)
