# Snippets

My snippets - adopted from friendly-snippets.

## Install

Use your plugin manager of choice, e.g.

### With Lazy.nvim

```lua
{ "andrewjmcgehee/snippets.nvim" }
```

> [!WARNING]
> If you're using LuaSnip make sure to use
> `require("luasnip.loaders.from_vscode").lazy_load()`, and add
> `andrewjmcgehee/snippets.nvim` as a dependency for LuaSnip, otherwise snippets might not
> be detected. If you don't use `lazy_load()` you might notice a slower
> startup-time
>
> ```lua
> {
>   "L3MON4D3/LuaSnip",
>   dependencies = { "andrewjmcgehee/snippets.nvim" },
> }
> ```
