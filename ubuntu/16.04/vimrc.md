" 让 ~/.vimrc 文件保存后, 配置变更立即生效  
autocmd BufWritePost $MYVIMRC source $MYVIMRC

" 定义快捷键的前缀,即<Leader>  
let mapleader=";"

"基于autoindent的一些改进  
set smartindent

"设置一个 tab 显示出来是多少个空格的长度，默认8  
set tabstop=4

"表示在编辑模式的时候按退格键的时候退回缩进的长度，当 set expandtab  
"的时候如果你不设置这个选项的时候，你就知道痛苦了，你必须一格一格的往前删除，  
"如果设置了这个选项的话，就可以一次就往前删除指定个数的空格  
set softtabstop=4

"表示当缩进的时候，每一级的缩进长度  
set shiftwidth=4

"这个设置表示缩进用空格来表示，noexpandtab 则是用制表符表示一个缩进。  
set expandtab

"显示当前光标的行列信息  
set ruler

"设置检索  
set ignorecase
set smartcase
set incsearch 
set hlsearch

" 光标离窗口上下边界的最小行距为多少时会引起窗口滚动  

set so=5

"启用鼠标  
set mouse=a

"启用行号  
set nu 

" 设置光标所在行和列的提示  
set cursorline
set cursorcolumn

"使得非可见字符用特殊的字符显示出来  
set list
set listchars=tab:>>,eol:¬

"非可见字符 eol extends precedes 是由 NonText 高亮组来控制显示颜色的  
hi NonText ctermfg=239

"nbsp tab trail 是由 SpecialKey 高亮组来定义颜色的  
hi SpecialKey ctermfg=239

"显示在命令模式下输入的完整的命令  
set showcmd

"设置有两行状态栏(一行状态，一行命令)，默认状态下两行和并在一起  
set laststatus=2

" save and restore folds when a file is closed and re-opened  
autocmd BufWinLeave *.* mkview  
autocmd BufWinEnter *.* silent loadview 

"当移动光标的时候，检测文件内容是否已经改变，提示 reload 文件内容  
au CursorMoved * checktime

nnoremap <c-h> <C-w>h  
nnoremap <c-l> <C-w>l  
nnoremap <c-k> <C-w>k  
nnoremap <c-j> <C-w>j  

" 开启文件类型侦测  
filetype on

" 根据检测到的不同类型加载相应的插件  
filetype plugin on

"使用缩进定义文件  
filetype indent on

"复制功能  
nnoremap <Leader>p "+p  
vnoremap <Leader>y "+y

"取消高亮搜索  
noremap <F2> :nohlsearch<CR>

"保存文件或保存并退出快捷键设置  
inoremap <c-s> <esc>:w<cr>a  
nnoremap <c-s> :w<cr>  
inoremap <c-a> <esc>:wq<cr>  
nnoremap <c-a> <esc>:wq<cr>  
inoremap <c-x> <esc>:q<cr>  
nnoremap <c-x> <esc>:q<cr>  
