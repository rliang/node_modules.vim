# node_modules.vim
Vim plugin that hosts a node_modules directory.

## Summary
Some vim plugins rely on external executables which are provided by npm
modules, which are usually installed either globally or per-project. This
plugin enables a vim-wide node_modules directory, adding its `bin`
subdirectory to `$PATH`.

## Example
With vim-plug:
```vim
let modules = 'eslint coffee-script'
Plug 'rliang/node_modules.vim' {'do': 'npm i ' . modules}
```
Then just run `PlugUpdate!` each time you add a new module.

## Variables
* `g:node_modules`: The absolute path of the `node_modules` directory.
