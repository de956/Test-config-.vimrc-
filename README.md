###### This one contains the following additions:

vim-plug  https://github.com/junegunn/vim-plug <br />
nerdtree  https://github.com/scrooloose/nerdtree <br />
YouCompleteMe https://github.com/ycm-core/YouCompleteMe <br />
auto-pairs https://github.com/jiangmiao/auto-pairs <br />
vim-gitgutter https://github.com/airblade/vim-gitgutter <br />
vim-fugitive https://github.com/tpope/vim-fugitive <br />
ctrlp.vim https://github.com/kien/ctrlp.vim <br />
vim-ruby https://github.com/vim-ruby/vim-ruby <br />
emmet-vim https://github.com/mattn/emmet-vim  <br />
gruvbox  (colorschemes) https://github.com/morhetz/gruvbox

###### Settings:

colorscheme gruvbox
set background=dark  <br />
set number  <br />
set hlsearch  <br />
set incsearch  <br />
syntax on

###### Quick setup (using Ubuntu 16.04 and later):

Download / copy the .vimrc file to your home directory 

Run the following command in the terminal to install the plugin manager:  <br />

<pre>curl -fLo <span class="pl-k">~</span>/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim</pre>
  
 More info about the plugin manager [vim-plug](https://github.com/junegunn/vim-plug)  <br />
 
 Run vim, execute:  <br />
 
 `:PlugUpdate`  <br />
 `:PlugInstall`  <br />
 
 You can also use the command: <br />
 
 `:source ~/.vimrc`
 
Error in vim:

<pre><code>YCM core library not de...you need to compile YCM before using it. Follow the instructions in the documentation</code></pre>

Error in the terminal:

>YouCompleteMe unavailable: requires Vim compiled with Python (2.7.1+ or 3.5.1+) support. <br />
>Press ENTER or type command to continue

###### Fix error vim / terminal 

Run a command in the terminal:  <br />

`sudo apt install build-essential cmake python3-dev`

Compiling YCM without semantic support for C-family languages: (:exclamation: Notice! Compilation may take a long time :exclamation:) <br />

`cd ~/.vim/plugged/YouCompleteMe` <br />
`python3 install.py`  <br />

More info about [YouCompleteMe](https://github.com/ycm-core/YouCompleteMe#linux-64-bit)

###### If you need a Vim editor for MC (midnight commander), then type in the terminal: <br />

`select-editor`

Select a number and press enter: <br />

> Select an editor.  To change later, run 'select-editor'.
>  1. /bin/nano        <---- easiest
>  2. /usr/bin/vim.basic
>  3. /usr/bin/mcedit
>  4. /usr/bin/vim.tiny
>  5. /bin/ed
>
> Choose 1-5 [1]: 2

