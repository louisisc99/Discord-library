# Discord-library
-- Load the DiscordLib UI Library
-- Credit: dawid#7205 (https://github.com/dawid-scripts/UI-Libs)
local DiscordLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/dawid-scripts/UI-Libs/main/discord%20lib.txt"))()

-- Create the main window
local win = DiscordLib:Window("My Discord UI")

-- Add a server (tab) called "Main Server"
local mainServer = win:Server("Main Server", "http://www.roblox.com/asset/?id=6031075938")

-- Add a channel (sub-tab) called "Actions"
local actionsChannel = mainServer:Channel("Actions")

-- Add a button to the "Actions" channel
actionsChannel:Button("Greet", function()
    DiscordLib:Notification("Notification", "Hello, world!", "Got it!")
end)

-- Add a toggle to enable or disable features
actionsChannel:Toggle("Enable Cool Feature", false, function(state)
    if state then
        print("Cool feature enabled!")
    else
        print("Cool feature disabled!")
    end
end)

-- Add a channel (sub-tab) called "Settings"
local settingsChannel = mainServer:Channel("Settings")

-- Add a slider to control a value
local slider = settingsChannel:Slider("Adjust Volume", 0, 100, 50, function(value)
    print("Volume set to:", value)
end)

-- Add a button to reset the slider
settingsChannel:Button("Reset Volume", function()
    slider:Change(50)
end)

-- Add a dropdown for selecting options
local dropdown = settingsChannel:Dropdown("Select Option", {"Option 1", "Option 2", "Option 3"}, function(option)
    print("Selected:", option)
end)

-- Add buttons to manage the dropdown
settingsChannel:Button("Clear Options", function()
    dropdown:Clear()
end)

settingsChannel:Button("Add New Option", function()
    dropdown:Add("New Option")
end)

-- Add a channel (sub-tab) called "About"
local aboutChannel = mainServer:Channel("About
