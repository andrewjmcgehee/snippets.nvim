# Snippets

## Install

Use your plugin manager of choice, e.g.

### With Lazy.nvim

```lua
{ "andrewjmcgehee/snippets.nvim" }
```

> [!WARNING]
> If you're using LuaSnip make sure to use
> `require("luasnip.loaders.from_vscode").lazy_load()`, and add
> `friendly-snippets` as a dependency for LuaSnip, otherwise snippets might not
> be detected. If you don't use `lazy_load()` you might notice a slower
> startup-time
>
> ```lua
> {
>   "L3MON4D3/LuaSnip",
>   dependencies = { "andrewjmcgehee/snippets.nvim" },
> }
> ```

## Usage

This collection of snippets should work with any snippet engine that supports
loading vscode snippets. Like for example:

- [vim-vsnip](https://github.com/hrsh7th/vim-vsnip)
- [LuaSnip](https://github.com/L3MON4D3/LuaSnip)
- [coc-snippets](https://github.com/neoclide/coc-snippets)

## Add snippets from a framework to a filetype.

> [!NOTE]
> This is handled by your snippet engine and has nothing to do with this snippets collection

There's extra snippets included in this repo but they are not added by default,
since it would be irrelevant for people not using those frameworks. See
[`snippets/frameworks`](https://github.com/andrewjmcgehee/snippets.nvim/tree/main/snippets/frameworks)

For example: if you want to add rails snippets to ruby.

With LuaSnip:

```lua
require'luasnip'.filetype_extend("ruby", {"rails"})
```

## Excluding snippets

> [!NOTE]
> This is handled by your snippet engine and has nothing to do with this snippets collection

With LuaSnip, see `help luasnip-loaders`

```lua
-- will exclude all javascript snippets
require("luasnip.loaders.from_vscode").load {
    exclude = { "javascript" },
}
```

## Showcase

### HTML

![HTML gif](https://user-images.githubusercontent.com/67771985/131255337-d53f3408-b60d-44a2-93ba-9a3240a7436e.gif)

### JS

![JS gif](https://user-images.githubusercontent.com/67771985/131255342-e393165a-e4b1-401e-9084-a782b9dd3fef.gif)
