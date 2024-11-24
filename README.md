
# DiscordLib Example

This repository demonstrates how to use the **DiscordLib** library for creating Discord-style GUIs in Roblox.

## Example Code:

```lua
local DiscordLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/dawid-scripts/UI-Libs/main/discord%20lib.txt"))()
local win = DiscordLib:Window("My UI")
local serv = win:Server("Main Server", "")
local btns = serv:Channel("Buttons")
btns:Button("Kill all", function()
    DiscordLib:Notification("Notification", "Killed everyone!", "Okay!")
end)
