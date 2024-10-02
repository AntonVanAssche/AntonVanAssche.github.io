+++
title = 'Date Time Inserter'
date = 2022-12-31
+++

## Description

Date Time Inserter is a simple/basic Neovim plugin that allows you to easily
insert the current date and time into your Neovim buffer.

This plugin does basically the same as the code block below, but this requires
the date command to be installed on the system. Therefore it's not always
possible to use it on every system, this is exactly what Date Time Inserter
tries to solve by using the lua built-in os.date() function. The plugin allows
you to insert the date and time into your Neovim buffer on every system
regardless of the operating system.

```lua
vim.keymap.set(
    "n",
    "<leader>dt",
    ':r! date "+\\%d-\\%m-\\%Y" <CR>',
    {noremap = true, vim.keymap.set}
)
vim.keymap.set(
    "n",
    "<leader>tt",
    ':r! date "+\\%H:\\%M:\\%S" <CR>',
    {noremap = true, vim.keymap.set}
)
```

## Demo

![Date Time Inserter Demo](https://github.com/AntonVanAssche/date-time-inserter.nvim/raw/master/assets/preview.gif?raw=true)

## Features

- [1] Insert the current date.
- [2] Insert the current time.
- [3] Customizable date and time format.
- [4] Customizable keybindings.

## Links

- [1] GitHub: <https://www.github.com/AntonVanAssche/date-time-inserter.nvim>
