# ⚠ I DID NOT MAKE THIS ⚠
### All credits go to liammuwu on v3rmillion ([https://v3rmillion.net/member.php?action=profile&uid=2406463](https://v3rmillion.net/member.php?action=profile&uid=2406463))
# Hyphon UI Library Reupload
### Simple reupload of UI library from https://v3rmillion.net/showthread.php?tid=1203835

## Library info
```
Author: liammuwu
Supported executors: Synapse X, Synapse V3, (?) Scriptware *all untested for now*
Type: Drawing
```

## Preview:
![preview](https://raw.githubusercontent.com/scotdotwtf/Hyphon-UI-Library-Reupload/main/Hyphon_Preview.png)

## Library Demo
- ### Unfinished demo, more soon whenever synapse is unpatched
```lua
local Hyphon = loadstring(game:HttpGet("https://raw.githubusercontent.com/scotdotwtf/Hyphon-UI-Library-Reupload/main/Hyphon_Library.lua"))({cheatname = 'cheat name', gamename = "game name"})
```

## Documentation
- ### More documentation will be made later, this is just pasted from v3rm

```lua
-- documentation
option:set_enabled(enabled <boolean>)
option:set_text(text <string>)

-- menu
local menu = library:create('menu', properties <table>)
library.menu = menu

text <string>
size <udim2>
position <udim2>


-- tab
local tab = menu:tab(properties <table>)

text <string>
order <number>

-- section
local section = tab:section(properties <table>)

text <string>
side <number>


-- toggle
local toggle = section:toggle(properties <table>)

default <boolean>
text <string>
order <number>
enabled <boolean>
callback <function>


-- slider
local slider = section:slider(properties <table>)
local slider = toggle:slider(properties <table>)

default <number>
min <number>
max <number>
increment <number>
text <string>
order <number>
enabled <boolean>
callback <function>


-- colorpicker
local colorpicker = section:colorpicker(properties <table>)
local colorpicker = toggle:colorpicker(properties <table>)

default <color3>
default_opacity <number>
text <string>
order <number>
enabled <boolean>
callback <function> [color, opacity]


-- keybind
local keybind = section:keybind(properties <table>)
local keybind = toggle:keybind(properties <table>)

default <keycode> <userinputtype>
mode <string> [toggle, hold, always]
text <string>
order <number>
enabled <boolean>
callback <function>


-- textbox
local textbox = section:textbox(properties <table>)
local textbox = toggle:textbox(properties <table>)

default <string>
placeholder <string>
text <string>
order <number>
enabled <boolean>
callback <function>

-- button
local button = section:button(properties <table>)

text <string>
order <number>
enabled <boolean>
callback <function>

-- separator
local separator = section:separator(properties <table>)

text <string>
order <number>
enabled <boolean>
```
