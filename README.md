# node_modules.vim
Vim plugin that hosts a node_modules directory.

## Summary
Some vim plugins rely on npm modules, which can be installed either globally or
per-project. This plugin enables a vim-wide node_modules directory, adding its
`bin` subdirectory to `$PATH`.

## Example
With vim-plug:
```vim
let modules = 'eslint tern'
Plug 'rliang/node_modules.vim' {'do': 'npm i ' . modules}
```
Then just run `PlugUpdate!` each time you add a new module.

## Variables
* `g:node_modules`: The absolute path of the `node_modules` directory.
