# Fluent UI
### Made By 5awid, Showcase On [Youtube](https://youtu.be/jp8QcBoEzdc?si=OZgiNBESrSHq7irs), Icons On [Lucide](https://lucide.dev/icons)
## 🔌 Installation
#### Loadstring (Needed)
```lua
local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()
local SaveManager = loadstring(game:HttpGet("https://raw.githubusercontent.com/dawid-scripts/Fluent/master/Addons/SaveManager.lua"))()
local InterfaceManager = loadstring(game:HttpGet("https://raw.githubusercontent.com/dawid-scripts/Fluent/master/Addons/InterfaceManager.lua"))()
```
#### Window (Needed)
```lua
local Window = Fluent:CreateWindow({
    Title = "Fluent", -- Name of script
    SubTitle = "by dawid", -- Sub Title
    TabWidth = 160, -- Width of Tabs
    Size = UDim2.fromOffset(580, 460), -- Size of UI
    Acrylic = true, -- The blur may be detectable, setting this to false disables blur entirely
    Theme = "Dark",
    MinimizeKey = Enum.KeyCode.LeftControl -- Used when theres no MinimizeKeybind, When pressing pressing the key Leftctrl, it will show or not show the UI lib.
})
```
#### Tabs
```lua
local Tabs = {
    Main = Window:AddTab({ Title = "Main", Icon = "" }), -- Icon Means What Icon You Want in the tab, for example, Icon = "Home"
    Settings = Window:AddTab({ Title = "Settings", Icon = "settings" })
}
```
#### Dialog
```lua
Window:Dialog({
                Title = "Title",
                Content = "This is a dialog",
                Buttons = {
                    {
                        Title = "Confirm",
                        Callback = function()
                            print("Confirmed the dialog.")
                        end
                    },
                    {
                        Title = "Cancel",
                        Callback = function()
                            print("Cancelled the dialog.")
                        end
                    }
                }
            })
        end
```
## ⚡ Elements
#### Adding Buttons
```lua
Tabs.Main:AddButton({
        Title = "Button",
        Description = "Very important button",
        Callback = function()
    print("Button")
})
```
