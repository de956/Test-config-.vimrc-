This one contains the following additions:

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

Settings:

colorscheme gruvbox
set background=dark  <br />
set number  <br />
set hlsearch  <br />
set incsearch  <br />
syntax on

Quick setup (using Ubuntu 16.04 and later):

Download / copy the .vimrc file to your home directory 

Run the following command in the terminal to install the plugin manager:  <br />

`curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim`  <br />
  
 More info about the plugin manager 'vim-plug' https://github.com/junegunn/vim-plug  <br />
 
 Run vim, execute:  <br />
 
 `:PlugUpdate`  <br />
 `:PlugInstall`  <br />
 
On error:
<pre><code>YCM core library not de...you need to compile YCM before using it. Follow the instructions in the documentation</code></pre>
Run a command in the terminal:  <br />

`sudo apt install build-essential cmake python3-dev`

Compiling YCM without semantic support for C-family languages: <br />

`cd ~/.vim/plugged/YouCompleteMe
python3 install.py`  <br />

More info about YouCompleteMe add-on: https://github.com/ycm-core/YouCompleteMe#linux-64-bit
