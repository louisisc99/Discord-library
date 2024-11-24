# DiscordLib UI Library for Roblox

## Welcome to the **DiscordLib UI Library** for Roblox!

This repository provides a robust, user-friendly library for creating Discord-style GUIs within Roblox. If you want to integrate buttons, toggles, sliders, dropdowns, and more in your Roblox game, this library is for you! This document will explain how to get started, use each feature, and give you ready-to-copy code examples.

---

## Table of Contents

1. [How to Load the Library](#how-to-load-the-library)
2. [How to Create a Window](#how-to-create-a-window)
3. [How to Add a Server](#how-to-add-a-server)
4. [How to Add UI Elements](#how-to-add-ui-elements)
    - [Buttons](#how-to-add-a-button)
    - [Toggles](#how-to-add-a-toggle)
    - [Sliders](#how-to-add-a-slider)
    - [Dropdowns](#how-to-add-a-dropdown)
    - [Colorpickers](#how-to-add-a-colorpicker)
    - [Textboxes](#how-to-add-a-textbox)
    - [Key Binds](#how-to-add-key-binds)
    - [Labels](#how-to-add-labels)
5. [How to Use Sliced Edges (Rounded Corners)](#how-to-use-sliced-edges-rounded-corners)
6. [Credits](#credits)

---

## How to Load the Library

To use **DiscordLib**, you need to load it in your Roblox script. Use the following line of code to load the library:

```lua
-- Load the DiscordLib UI library
local DiscordLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/dawid-scripts/UI-Libs/main/discord%20lib.txt"))()
