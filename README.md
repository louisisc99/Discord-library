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
local DiscordLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/dawid-scripts/UI-Libs/main/discord%20lib.txt"))()
```
Window 
```lua
local win = DiscordLib:Window("My Discord UI")
```
servers
```lua
local mainServer = win:Server("Main Server", "http://www.roblox.com/asset/?id=6031075938")
local actionsChannel = mainServer:Channel("Actions")
```
buttons
```lua
actionsChannel:Button("Greet", function()
    DiscordLib:Notification("Notification", "Hello, world!", "Got it!")
end)
```
toggles
```lua
actionsChannel:Toggle("Enable Cool Feature", false, function(state)
    if state then
        print("Cool feature enabled!")
    else
        print("Cool feature disabled!")
    end
end)
```
Slider
```lua
local slider = actionsChannel:Slider("Adjust Volume", 0, 100, 50, function(value)
    print("Volume set to:", value)
end)
```
dropdowns 
```lua
local dropdown = actionsChannel:Dropdown("Select Option", {"Option 1", "Option 2", "Option 3"}, function(option)
    print("Selected:", option)
end)
```
Colorpicker 
```lua
local colorPicker = actionsChannel:Colorpicker("ESP Color", Color3.fromRGB(255, 1, 1), function(color)
    print("Selected color:", color)
end)
```
Textboxes 
```lua
local textbox = actionsChannel:Textbox("Enter Gun Power", "Type here!", true, function(input)
    print("User input:", input)
end)
```
label 
```lua
actionsChannel:Label("This is just a label.")
```
