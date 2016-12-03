# vimterm

![](https://cdn.rawgit.com/wvffle/vimterm/screenshots/waff%40nyarch.png)

vimterm provides simple window with neovim's :terminal at the bottom of the screen.

But why? That's a good question. vimterm lets you operate with your files and have a single terminal window attached to the bottom of your workspace.
For example, you can create a mapping to compile c++ programs with g++ without leaving your best editor.

Example mappings could look like this:

```
nnoremap <F4> :call vimterm#exec('g++ ' . expand('%') . ' -o /tmp/out') <CR>
nnoremap <F5> :call vimterm#exec('/tmp/out') <CR>
```

