---
title: moar or moor
pubDate: '2025-08-18'
---
# Modern pager

`moar`[^1] is command line replacement for the venerable tools `less` and `more`. These tools are known as pagers - they take a stream of text input and show it one page at a time, allowing you to read, scroll up and down, or even search through the text.

## Suprising warning

This morning, after running `brew update`, I settled in to explore the dark corners of some old infrastructure code. I frequently use `rg $STRING | moar` to find relationships across files.

But this time, a warning flashed: `moar` would soon be renamed to `moor`.

## Naming confusion

The name was already great, right? `moar` is clever and funny. Digging into why this familiar utility was changing, it turns out that Debian already has a package with a binary named `moar`. Debian and derivative linux distros like Ubuntu do not allow packages to publish a binary with the same name. So, in order to get `moar` into the `apt` package repositories, it would be simpler to rename the tool completely.[^2]

[^1]: moor on GitHub: https://github.com/walles/moor really long 
[^2]: Pull request to change the name: https://github.com/walles/moor/pull/305
