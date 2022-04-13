---
layout: post
title:  "Vim Cheatsheet"
author: 0xDipzy
tags: vim tutorial
---

| --- | --- |
| `:e` | Open and edit file |
| `[n] gg` | Go to line |
| `G` | Go to last line |
| `[n] o` | Open `n` new lines. `O` opens new line before current line |
| `u` | Undo |
| `Ctrl-r` | Redo |
| `Ctrl-o` | Switch from insert mode to normal mode for one command |
| `Shift-$` | Jump to end of line |
| `Shift-^` | Jump to start of line |
| `:set nonu` | Stop showing line numbers |
| `:set nu` | Show line numbers |

## Buffers

| --- | --- |
| `:ls` | List all buffers |
| `:bd` | Kill buffer |
| `[n] Ctrl-^` | Jump to buffer |

## Cut / Copy / Paste

| --- | --- |
| `d` | Delete/cut |
| `dd` | Delete current line |
| `diw` | Delete word at cursor |
| `Ctrl-u` | Delete from cursor to start of line |
| `c` | Delete and enter insert mode |
| `y` | Yank/copy |
| `yy` | Yank current line |
| `p` | Paste |
| `"[n]p` | Paste from register n |
| `:registers` | View registers |

## Search / Substitute

| --- | --- |
| `/foo` | Search "foo". Press n/N to toggle between next/previous occurrence |
| `:s/foo/bar` | Substitute first occurrence of "foo" with "bar" in current line |
| `:s/foo/bar/g` | Substitute all occurrences of "foo" with "bar" in current line |
| `:%s/foo/bar/g` | Substitute all occurrences of "foo" with "bar" in all lines|
| `:%s/foo/bar/gc` | Substitute all occurrences of "foo" with "bar" in current line with confirmation |

## Scrolling

| --- | --- |
| `Ctrl-u` | Scroll up half a screen |
| `Ctrl-d` | Scroll down half a screen |
| `Ctrl-f` | Scroll down one screen length |
| `Ctrl-b` | Scroll up one screen length |

## Windows

| --- | --- |
| `Ctrl-w v` | Split windows vertically |
| `Ctrl-w s` | Split windows horizontally |
| `Ctrl-w c` | Close window but keep buffer |
| `Ctrl-w o` | Close all other windows |
| `Ctrl-w right arrow` | Move cursor to window on the right |

## Autocomplete

| `Ctrl-p` | Prompt autocomplete / scroll up |
| `Ctrl-n` | Scroll down |
| `Ctrl-y` | Accept current choice |
| `Ctrl-e` | Exit menu |
