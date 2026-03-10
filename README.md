# dotfiles

My personal Neovim configuration, built with Lua. Optimized for fast navigation and a minimal editing experience.

## Plugins

- **[Telescope](https://github.com/nvim-telescope/telescope.nvim)** — Fuzzy finder for files, grep, and more
- **[Harpoon](https://github.com/ThePrimeagen/harpoon)** — Quick file switching between marked files
- **[Treesitter](https://github.com/nvim-treesitter/nvim-treesitter)** — Syntax highlighting and code parsing
- **[LSP](https://github.com/neovim/nvim-lspconfig)** — Language server protocol support
- **[Packer](https://github.com/wbthomason/packer.nvim)** — Plugin manager

## Structure

```
├── init.lua                      # Entry point
├── lua/diegorosales/
│   ├── init.lua                  # Core configuration loader
│   ├── set.lua                   # Vim options and settings
│   ├── remap.lua                 # Key remappings
│   └── packer.lua                # Plugin declarations
└── after/plugin/
    ├── colors.lua                # Colorscheme config
    ├── telescope.lua             # Telescope config
    ├── harpoon.lua               # Harpoon config
    ├── treesitter.lua            # Treesitter config
    └── lsp.lua                   # LSP config
```

## Installation

```bash
# Back up existing config
mv ~/.config/nvim ~/.config/nvim.bak

# Clone this repo
git clone https://github.com/dvrosalesm/dotfiles.git ~/.config/nvim

# Open Neovim and install plugins
nvim +PackerSync
```

Based on [ThePrimeagen's dotfiles](https://github.com/ThePrimeagen/.dotfiles).
