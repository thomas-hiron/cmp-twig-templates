# cmp-twig-templates

### ⚠️  This repo has been moved ⚠️

This code has been merged to https://github.com/thomas-hiron/cmp-symfony.

---

[nvim-cmp](https://github.com/hrsh7th/nvim-cmp) source for twig templates
located in project directory /templates.  

[FD](https://github.com/sharkdp/fd) is a required dependency.

Templates are refreshed every 30 seconds.

## Setup

```lua
require('cmp').setup({
  sources = {
    { name = 'twig_templates' },
  },
})
```

## Triggers

The plugin is activated for `php` and `twig` filetypes.  
The trigger character is a single quote, and the line must contains
`render` or `include`. This covers most of Symfony and twig
functions used to generate URLs:
- PHP
  - render
  - renderView
- Twig
  - include

## Configuration

There is no configuration at the moment.
