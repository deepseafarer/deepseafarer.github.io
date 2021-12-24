---
layout: post
title:  "Vim Cheatsheet"
author: 0xDipzy
tags: vim tutorial
---
| --- | --- |
| `:e` | Open and edit file |
| `dd` | Delete/cut current line |
| `[n] gg` | Go to line |
| `G` | Go to last line |
| `[n] o` | Open `n` new lines. `O` opens new line before current line |
| `u` | Undo |
| `Ctrl-r` | Redo |
| `Ctrl-o` | Switch from insert mode to normal mode for one command |
  

## Buffers

| --- | --- |
| `:ls` | List all buffers |
| `:bd` | Kill buffer |
| `[n] Ctrl-^` | Jump to buffer |


## Delete

| --- | --- |
| `d` | Delete/cut |
| `daw` | Delete word at cursor |
| `Ctrl-u` | Delete from cursor to start of line |


## Search / Substitute

| --- | --- |
| `/foo` | Search "foo". Press n/N to toggle between next/previous occurrence |
| `:s/foo/bar` | Substitute first occurrence of "foo" with "bar" in current line |
| `:s/foo/bar/g` | Substitute all occurrences of "foo" with "bar" in current line |
| `:%s/foo/bar/g` | Substitute all occurrences of "foo" with "bar" in all lines|
| `:%s/foo/bar/gc` | Substitute all occurrences of "foo" with "bar" in current line with confirmation |


## Windows

| --- | --- |
| `Ctrl-w v` | Split windows vertically |
| `Ctrl-w s` | Split windows horizontally |
| `Ctrl-w c` | Close window but keep buffer |
| `Ctrl-w o` | Close all other windows |
| `Ctrl-w right arrow` | Move cursor to window on the right |