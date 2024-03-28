# Abyss UI
This documentation is for Abyss UI Credit To The Owner

## Booting the Abyss UI Library
```lua
local Ui = loadstring(game:HttpGet("https://raw.githubusercontent.com/drillygzzly/Other/main/abyssoruce%40eayz.lua"))()
local Ui = Library
```




## Creating a Abyss UI Window
```lua
local Window = Library.CreateLib("TITLE", "DarkTheme")
```

## Creating a Load Time
```lua
local LoadTime = tick()
```

## Creating a Loader
```lua
local Loader = Library.CreateLoader(
    "Title Here", 
    Vector2.new(300, 300)
)
```

## Creating a Window
```lua
local Window = Library.Window(
    "Text Here", 
    Vector2.new(500, 620)
)
```

## Creating a Notify
```lua
Window.SendNotification(
    "Normal", -- Normal, Warning, Error 
    "Press RightShift to open menu and close menu!", 
    10
)
```

## Creating a Water Mark
```lua
Window.Watermark(
    "Text Here"
)
```

## Creating a Toggle
```lua
Section1:Toggle({
    Title = "Toggle1", 
    Flag = "Toggle_1",
    Type = "Dangerous",
    Callback = function(v)
        print("Value = "..v)
    end
}):
```

## Creating a Toggle Keybind
```lua
-- Toggle Keybind Below
    Keybind({
    Title = "KeybindToggle1",
    Flag = "Keybind_Toggle_1", 
    Key = Enum.UserInputType.MouseButton2, 
    StateType = "Toggle"
})
```

## Creating a Color Picker
```lua
}):
Colorpicker({
    Color = Library.Theme.Accent[2], 
    Flag = "Toggle2Color"
})
```

## Creating a Slider
```lua
Section1:Slider({
    Title = "Slider1", 
    Flag = "Slider_1", 
    Symbol = "", 
    Default = 0, 
    Min = 0, 
    Max = 20, 
    Decimals = 1,
    Callback = function(v)
        print("Value = "..v)
    end
})
```

## Creating Dropdown
```lua
Section1:Dropdown({
    Title = "Dropdown1", 
    List = {"1", "2" ,"3"}, 
    Default = "1", 
    Flag = "DropDown_1",
    Callback = function(v)
        print("Value = "..v)
    end
})
```

## Creating a Button
```lua
Section1:Button({
    Title = "Button1",
    Callback = function()
        print("Pressed!")
    end
})
```

## Creating a Label
```lua
--Section1:Label({
    --Title = "Label1"
--})
```

## Tab Player List
```lua
--Tab1:AddPlayerlist()
Window:AddSettingsTab()
Window:SwitchTab(Tab1)
Window.ToggleAnime(false)
LoadTime = math.floor((tick() - LoadTime) * 1000)
```
