# nvim-config

## My nvim configuration in Lua

1. Install [Nerd Fonts](https://www.nerdfonts.com/) (*ttf-nerd-fonts-symbols* in Arch distributions);

2. Clone repo into ~/.config/nvim;

3. *git clone --depth 1 https://github.com/wbthomason/packer.nvim ~/.config/nvim/site/pack/packer/start/packer.nvim*;

5. *:PackerInstall* in nvim;

6. Uncomment in *init.lua*:
~~~lua
require('nvim-tree').setup{}

require('lualine').setup {
  options = {
    theme = 'dracula-nvim'
  }
}
require('nvim-autopairs').setup{}
~~~
7. Uncomment in *lua/opts.lua*:
~~~lua
cmd('colorscheme dracula')
~~~
