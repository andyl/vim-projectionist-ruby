# vim-projectionist-ruby

Vim file navigation for Ruby projects 

This plugin supplies quick-nav links for Ruby projects.  **Alternate File
Navigation** gives commands to jump between an Ruby source file and it's
associated test.  **Related File Navigation** gives commands to jump between
Rails controllers, views and templates.

Install using `Plug` in your `.vimrc`:

    Plug 'tpope/vim-projectionist'
    Plug 'andyl/fuzzy-projectionist.vim'
    Plug 'andyl/vim-projectionist-ruby'

See also:
- tpope's [vim-projectionist][l1] plugin.  
- andyl's [fuzzy-projectionist.vim][l2] plugin.

## Alternate File Navigation

'Alternates' are the source code and test file - a one-to-one relationship.

`:A` - open the 'alternate' file

`:AS` - open the 'alternate' file in a split window

`:AV` - open the 'alternate' file in a vertical split window

`:AT` - open the 'alternate' file in another tab

## Related File Navigation

In Rails projects, you can jump between 'related' files (controllers /
templates / views).

There are two types of relations:
1) one-to-one relationship, eg `controller -> view`
2) one-to-many relationship, eg `controller => template`

For one-to-one relationships, use the Projectionist `E` commands:

- `:Econtroller`
- `:Eview`

For one-to-many relationships, use the Fuzzy-Projectionist `F` commands:

- `:Ftemplate`

[l2]: https://github.com/tpope/vim-projectionist
[l3]: https://github.com/andyl/fuzzy-projectionist.vim
