# cmp-luasnip-choice

[luasnip](https://github.com/L3MON4D3/LuaSnip) choice node completion source for [blink-cmp](https://github.com/saghen/blink.cmp)

## Installation

```lua
require("lazy").setup({
    {
        "becknik/blink-luasnip-choice",
        dependencies = {
            { "Saghen/blink.cmp" },
        },
        opts = {
            -- Optional config can go here
        }
    },
})
```

## Usage

```lua
require 'blink.cmp' .setup {
    -- …
    sources = {
        providers = {
            choice = {
                name = 'LuaSnip Choice Nodes',
                module = 'blink-cmp-luasnip-choice'
                opts = {},
            },
        }
    },
    -- …
    default = {
        'choice',
        'lsp',
        -- …
    }
}

```
