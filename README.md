setcolors.vim
=============

Change the color scheme from a list of color scheme names.

Shameless rip from http://vim.wikia.com/wiki/Switch_color_schemes#Script

# Install

Install via [Pathogen](https://github.com/tpope/vim-pathogen):

    cd ~/.vim/bundle
    git clone https://github.com/felixhummel/setcolors.vim.git setcolors

Install via [Vundle](https://github.com/VundleVim/Vundle.vim), add to `~/.vimrc`:

    Plugin 'axmac/setcolors.vim'

# Configure

Set color scheme names to use in .vimrc

    let g:mycolors=['slate', 'torte']

Set the list of color schemes used by the above (default is 'all'):

    :SetColors all              (all $VIMRUNTIME/colors/*.vim)
    :SetColors my               (names built into script)
    :SetColors blue slate ron   (these schemes)
    :SetColors                  (display current scheme names)

Set the current color scheme based on time of day:
  :SetColors now

Cycle through color schemes, press key:

- F8: next scheme
- Shift-F8: previous scheme
- Alt-F8: random scheme

# Acknowledgements

- Original at http://vim.wikia.com/wiki/Switch_color_schemes#Script
