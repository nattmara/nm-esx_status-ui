# Nattmara ES Extended Status User Interface
### nm-esx_status-ui
---

## About
Alternative approaches to present statuses from esx_status script.
Built with lua, vite + vuetify 3

## Dependencies
ESX & ESX_STATUS

This script is built for [ESX Framework, ESX Legacy](https://github.com/esx-framework "ESX Framework")
If not using the official ESX Framework version we can not guarantee that the script will work for you.

## User Todo:

1. Make sure to export esx_status GetStatusData - Minimal could be true

	Example on export in esx_status (Client side):

	```lua
	exports('getAll', function()
		return GetStatusData(true)
	end)
	```

	Add this export to the config in nm-esx_status-ui (Config.esx_status_export)
---

2. If having more statuses than default:
- Make sure to add Icon in Config.lua. Make sure to use the [MDI Icons](https://pictogrammers.com/library/mdi/, "MDI Icons")
![alt text](https://cdn.discordapp.com/attachments/1063025092663185429/1084173516158541834/image.png)

- Make sure to add to Locales.lua ["status"]-keys at all languages

![alt text](https://cdn.discordapp.com/attachments/1063025092663185429/1084173054738972693/image.png)


## FAQ
 > How do I open the configuration?

	/uiconfig command

> Can i reset the UI?
	
	You can use /uireset to reload the UI and fetch data from your storage once again

> Can i clear the UI settings?

	Yes, use /uiclear. This will clear the storage and reset all the settings to default.

> Where is the settings saved?

	 On client localStorage, which means it would be saved until they clear cache

> Is my settings automatically saved?

	No - on every page in the UI you got the Save-button which will save the settings to the localStorage. (Bar settings, Global Settings, Individual Settings)

>  I found a bug - what do I do?

	Make sure to declare it in official Nattmara Store Discord https://discord.gg/644Ha7jM

	If it's a bug, we will fix it.

> Will there be updates for the script?
	
	Bugs will always be prioritized and fixed.
	You can always check the package roadmap at Nattmara Store Official discord (https://discord.gg/644Ha7jM) if there is any else planned to be updated for the script.

## Showcase Video
<a href="http://www.youtube.com/watch?feature=player_embedded&v=wK8PJ6cQlzA
" target="_blank"><img src="http://img.youtube.com/vi/wK8PJ6cQlzA/0.jpg" 
alt="Showcase Video" width="240" height="180" border="10" /></a>

## Images
![alt text](https://cdn.discordapp.com/attachments/1063025092663185429/1063025144991326288/diff_style1.jpg)
![alt text](https://cdn.discordapp.com/attachments/1063025092663185429/1063025145192665098/diff_style2.jpg)
![alt text](https://cdn.discordapp.com/attachments/1063025092663185429/1063025145742106664/global_icons_settings.jpg)
![alt text](https://cdn.discordapp.com/attachments/1063025092663185429/1063025146006360094/individual_icons_settings.jpg)
![alt text](https://cdn.discordapp.com/attachments/1063025092663185429/1063025146245431296/status_bar_settings.jpg)
![alt text](https://cdn.discordapp.com/attachments/1063025092663185429/1063025146551607326/temporary.jpg)
