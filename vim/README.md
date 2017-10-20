# Installation

* copy the vimrc file to your ~/.vimrc
* open vim
* run **PluginInstall** in command mode
* install ag https://github.com/ggreer/the_silver_searcher (optional)
* you're good to go!

# Helpful stuff to get you started right away

## Searching files and tags

* press `Ctrl+p` to open the fuzzy file searcher
* default mode is file searcher
* enter the file you are searching for
* if you want to search for tags instead switch to tags via `Ctrl+f` / `Ctrl+b` (requires ctags file)

## Grepping the current project (no fuzzyiness)

* press `Ctrl+f` to search for word under the cursor
* or enter `CtrlSF <word>` in command mode

## Using the git plugin

I am not 100% happy with the way I currently use this plugin. It's a pretty powerful git wrapper, and would
require a bit more time to dig into. But I am ok with using git in the shell anyways =)

But as examples some of the stuff that I use:

### View history of a file

* `Glog` with current file to get history of current file
* then `copen` to open vim quickfix list
* use the quickfix list to go through revisions
* `Gdiff` or `vert diffsplit #` to show diff between selected revision and HEAD (?)

### Viewing last commits that changed lines of current file

* `Gblame` to list a the revision where the line was last touched
* move to the quickfix list and press `o` to open the diff/commit in a new window

# Stuff to check/todo

* check https://github.com/junegunn/fzf.vim => one plugin to do what ctrlp + ctrlsf is doing
* auto update ctags instead of on demand (i.e. branch switch)
* shell directly as sub window in vim? instead of using ctrl+z / fg combination (this picture looks tasty: [nice
  setup!](https://camo.githubusercontent.com/330721e34edb16976a8922f2978dfb6d7616071a/687474703a2f2f636c2e6c792f696d6167652f336b313731533345336b32712f53637265656e25323053686f74253230323031332d30322d3037253230617425323031312e30362e3431253230414d2e706e67))
* adjust colorscheme or try new colorscheme to have a nicer way to display line numbers (I currently don't like the way
  neodark does it)

# Notes

* trying out auto completion currently (http://github.com/valloric/youcompleteme) so you might want to remove that since
  it requires extra setup.
