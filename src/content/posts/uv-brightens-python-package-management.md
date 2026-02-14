---
title: uv brightens python package management
pubDate: '2025-08-19'
---

`uv`[^1] rapidly disrupted the Python package management space, showing that innovation is still possible in well established ecosystems - as long as it solves a real pain point.

[^1]: uv, https://github.com/astral-sh/uv - An extremely fast Python package and project manager, written in Rust.

# Use uv in an existing project

```
uv init .
uv add -r requirements.txt
uv run python main.py
```

# Manage python from uv

```
uv python install 3.13
```
