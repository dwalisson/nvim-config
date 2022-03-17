# nvim-config
My nvim configuration in Lua

1. Install [Nerd Fonts](https://www.nerdfonts.com/) (*ttf-nerd-fonts-symbols* in Arch distributions);

2. *git clone --depth 1 https://github.com/wbthomason/packer.nvim ~/.config/nvim/site/pack/packer/start/packer.nvim*;

4. *:PackerInstall* in nvim;

5. Uncomment in *init.lua*:
~~~lua
require('nvim-tree').setup{}

require('lualine').setup {
  options = {
    theme = 'dracula-nvim'
  }
}
require('nvim-autopairs').setup{}
~~~
6. Uncomment in *lua/opts.lua*:
~~~lua
cmd('colorscheme dracula')
~~~
