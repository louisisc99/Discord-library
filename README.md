
---

DiscordLib Roblox UI Library

Usage

Load the Library

local DiscordLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/dawid-scripts/UI-Libs/main/discord%20lib.txt"))()

Create the Main Window

local win = DiscordLib:Window("My UI")

Add a Server (Tab)

local server = win:Server("Main Server", "")

Add a Channel (Sub-tab)

local channel = server:Channel("Actions")

Add UI Elements

Button

channel:Button("Example Button", function()
    print("Button clicked!")
end)

Toggle

channel:Toggle("Example Toggle", false, function(state)
    print("Toggle state:", state)
end)

Slider

local slider = channel:Slider("Example Slider", 0, 100, 50, function(value)
    print("Slider value:", value)
end)

Dropdown

local dropdown = channel:Dropdown("Example Dropdown", {"Option 1", "Option 2"}, function(selection)
    print("Selected:", selection)
end)

Color Picker

channel:Colorpicker("Example Color Picker", Color3.new(1, 0, 0), function(color)
    print("Selected color:", color)
end)


---

This is the minimal, no-frills documentation. Just copy and paste the code to see the library in action!

Understood! Here’s the clean and straight-to-the-point documentation for your GitHub repository, with no unnecessary extras. This version is easy to read and focused solely on using the library.


---

DiscordLib Roblox UI Library

Usage

Load the Library

local DiscordLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/dawid-scripts/UI-Libs/main/discord%20lib.txt"))()

Create the Main Window

local win = DiscordLib:Window("My UI")

Add a Server (Tab)

local server = win:Server("Main Server", "")

Add a Channel (Sub-tab)

local channel = server:Channel("Actions")

Add UI Elements

Button

channel:Button("Example Button", function()
    print("Button clicked!")
end)

Toggle

channel:Toggle("Example Toggle", false, function(state)
    print("Toggle state:", state)
end)

Slider

local slider = channel:Slider("Example Slider", 0, 100, 50, function(value)
    print("Slider value:", value)
end)

Dropdown

local dropdown = channel:Dropdown("Example Dropdown", {"Option 1", "Option 2"}, function(selection)
    print("Selected:", selection)
end)

Color Picker

channel:Colorpicker("Example Color Picker", Color3.new(1, 0, 0), function(color)
    print("Selected color:", color)
end)


---
