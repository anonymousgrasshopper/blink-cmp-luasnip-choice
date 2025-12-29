# cmp-luasnip-choice

[luasnip](https://github.com/L3MON4D3/LuaSnip) choice node completion source for [nvim-cmp](https://github.com/hrsh7th/nvim-cmp)


https://user-images.githubusercontent.com/25270060/202857316-f6d13c97-7deb-4bfb-bb17-4937755b40cf.mp4


## Installation via [Packer](https://github.com/wbthomason/packer.nvim)

```lua
vim.api.nvim_create_autocmd("User", {
    pattern = "LuasnipChoiceNodeEnter",
    callback = function()
        vim.schedule(function()
            require("blink-cmp").show {
                providers = { "luasnip-choice" },
            }
        end)
    end,
})
```
