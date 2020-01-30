# esx_inventoryhud 2.1
Inventory HUD for ESX. You can open and close inventory using F2. Part of code was taken from [es_extended](https://github.com/ESX-Org/es_extended).

Developers By" [Emilia](https://github.com/Emilia-Dev) 
FiveM is a modification for Grand Theft Auto V [FiveM](https://fivem.net/)
### I don't allow to sell this script or pretended as yours even this script is not working.

## Requirements
* [es_extended](https://github.com/ESX-Org/es_extended)
* [pNotify](https://forum.fivem.net/t/release-pnotify-in-game-js-notifications-using-noty/20659)

# Discord 
<p align="center">
  <a href="https://discord.gg/BmvG9sm">
    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcToc0_EENZ5K4P6ZUQLMKlWsGBOoMO6LW5RXrX1lzJtmGp5QRxR&s?style=shield" alt="Discord Server">
  </a>
</p>
<p align="center">
  <a href="https://discordapp.com/api/oauth2/authorize?client_id=668032682348904458&permissions=1379391520&scope=bot">
    <img src="https://discordapp.com/api/guilds/133049272517001216/widget.png?style=shield" alt="Discord Server">
  </a>
</p>


## Features
- Drag and drop
- Using items
- Dropping items
- Giving items
- Cash included
- Accounts support (bank, black money, ...)
- Weapons support
- Fully configurable (check config.lua and html/js/config.js)
- Locale files included (check locales/ and html/locales/ directories)

## Addons
* [Vehicle trunk inventory](https://github.com/Trsak/esx_inventoryhud_trunk/tree/master)

## Screens
* [https://i.imgur.com/eHD01Tl.png](https://i.imgur.com/eHD01Tl.png)

## Download & Installation

### Using Git
```
cd resources
git clone https://github.com/Trsak/esx_inventoryhud [esx]/esx_inventoryhud
```

### Manually
- Download https://github.com/Trsak/esx_inventoryhud/archive/master.zip
- Put it in the `[esx]` directory

## Installation
- Open `es_extended`, then find and remove this code in `client/main.lua`:
```
-- Menu interactions
Citizen.CreateThread(function()
	while true do

		Citizen.Wait(0)

		if IsControlJustReleased(0, Keys['F2']) and IsInputDisabled(0) and not isDead and not ESX.UI.Menu.IsOpen('default', 'es_extended', 'inventory') then
			ESX.ShowInventory()
		end

	end
end)
```
- Add this to your `server.cfg`:

```
start esx_inventoryhud
```

## Config files
* config.lua
* html/js/config.js
