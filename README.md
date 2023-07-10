# resize.nvim
resize.nvim provides an intuitive way to resize windows using arrow keys. With Vim's native window resize shortcuts being less intuitive, this plugin allows you to easily adjust the size of windows using Ctrl + arrow key movements.

## Installation
[packer.nvim](https://github.com/wbthomason/packer.nvim) :
```lua
use {'0xm4n/resize.nvim'}
```

## Usage
Add this to your config:
```lua
vim.keymap.set("n", "<C-Left>", "<cmd>lua require('resize').ResizeLeft()<CR>", {silent=true})
vim.keymap.set("n", "<C-Right>", "<cmd>lua require('resize').ResizeRight()<CR>", {silent=true})
vim.keymap.set("n", "<C-Up>", "<cmd>lua require('resize').ResizeUp()<CR>", {silent=true})
vim.keymap.set("n", "<C-Down>", "<cmd>lua require('resize').ResizeDown()<CR>", {silent=true})

```
Using these mappings:

In normal mode, <kbd>\<C-Left\></kbd> will resize the current window to the left. <kbd>\<C-Right\></kbd> will resize the current window to the right...
