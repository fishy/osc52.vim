# osc52.vim

Vim/NeoVim plugin for OSC52

## Installation

Via [`vim-plug`](https://github.com/junegunn/vim-plug):

```vim
Plug 'fishy/osc52.vim'
```

Manually: Just copy `plugin/osc52.vim` to your vim/NeoVim's plugin directory.

## Usage

I use this mapping in my `~/.config/nvim/init.vim`:

```vim
" For osc52
vnoremap <leader>y y:call SendViaOSC52(getreg('"'))<cr>
```

## Acknowledgement

`plugin/osc52.vim` is forked from [Chromium's libapp project][orig-link],
with modifications to make it work for NeoVim.

[orig-link]: https://chromium.googlesource.com/apps/libapps/+/fde205949f9c1316baebd956a869bf754cc7e23f/hterm/etc/osc52.vim
