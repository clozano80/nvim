# nvim for ubuntu/debian - nvim 0.5.0 (not lua)
```
Personal nvim configuration:
With coc, prettier, nerdcomment,...
```

## Installation


- Install nvim nodejs and yarn 
  
  ``` 
  sudo apt install neovim nodejs yarn   #if node is over v.14
  
  # if ubuntu focal nodejs version 10.19... para node >= 14
   curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -
   sudo apt-get install -y nodejs


   # Using Debian, as root
   curl -fsSL https://deb.nodesource.com/setup_16.x | bash -
   apt-get install -y nodejs
      
  ```
  
- Install nerd font for icons https://github.com/ryanoasis/nerd-fonts
- create .config/nvim
copy files init.vim and coc .json to .config/nvim
- upload files
- alias vim="nvim"

- Install plug.vim if errors E117 (in neovim is like follows) 
```
 sh -c 'curl --insecure -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \                                                                https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
 
 #problems insecure certificates use --insecure
 
 sh -c 'curl --insecure -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \                                                                https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
 ```
 
```
if coc not installed properly or with coc#util#install needs to:
cd .vim/plugged/coc...
yarn install && yarn bild
or
npm install
```

```
Inside nvim/vim
:checkhealth "comprobamos que funciona
:PlugInstall 
:CocInstall <plugin si no está instalado>

:CocCommand #example snippets
:CocInstall coc-snippets
```

## Special key
```<space> espacio```
 
## Help Api autocomplete
```
<ctrl>+P
Shift K "show tooltip
:gd (go to definition)
F2 rename all files with...
```
## move between splits or windows
```
 <ctrl+w> <H,J,K,L>
<ctrl+w>W "next window
<ctrl+w>q  "quit
<ctrl+w>v/h split v or horizontal
<ctrl+w> <number optional> ><+-  # decrease or increase split window

<ctrl+b>b next open document (no tabs)
<ctrl+b>1..4 move between opened docs
```
 
## nredtree
 ```
ctrl+n
select file and "t" #Open in tab 
select file and "i" split Horz
select file and "v" split Vertical
```
 
## Comment
 ```
Visual mode select and <space>cc
++ Comenter toggle in visual
```
## terminal
 ```
<space>t
```
 
## next tab
 ```
ctrl+t
```
## Prettier
 ```
:Prettier or <ctrl+i>
```
 
## Search FZF
 ```
Ag requires The Silver Searcher (ag) sudo apt install silversearcher-ag
Rg requires ripgrep (rg) sudo apt install ripgrep

:Ag [PATTERN]	ag search result (ALT-A to select all, ALT-D to deselect all)
:Rg [PATTERN]	rg search result (ALT-A to select all, ALT-D to deselect all)
```
