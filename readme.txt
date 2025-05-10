-- EXAMPLE 



local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/BGIHT1717/Huiware-0lliware-/refs/heads/main/HuiWare%20ui"))()
local Window = Library:CreateWindow()

local MainTab = Window:CreateTab("Main")
MainTab:CreateButton("Button 1", function()
script
    print("Button 1 Clicked!")
end)

MainTab:CreateToggle("Toggle 1", function(state)
script
    print("Toggle State:", state)
end)

MainTab:CreateLabelButton("Label Info", "This is a large label text\nYou can add multiple lines here\nThis is an example text\nAdd more information as needed")

MainTab:CreateButton("Button 2", function()
script
    print("Button 2 Clicked!")
end)

local SettingsTab = Window:CreateTab("Settings")
SettingsTab:CreateButton("Settings Button", function()
    print("Settings Button Clicked!")
end)

SettingsTab:CreateToggle("Settings Toggle", function(state)
    print("Settings Toggle State:", state)
end)

SettingsTab:CreateLabelButton("Settings Info", "Settings Information\nCustomize this text\nAdd settings details here")
