# SpellShop_UI


##### About

A custom UI module for use by map makers
Version 1.01

##### Preview

Puu.sh links:
[Gold only](http://puu.sh/b4Owf/ffdf09b850.webm) | [Point only](http://puu.sh/b4Oyt/2e6ec6afd6.webm) | [Gold and point](http://puu.sh/b4OB0/f3a605cbdc.webm) | [Info tab](http://puu.sh/b2yJ1/950b2d3373.webm)

Youtube links:
[Gold only](https://www.youtube.com/watch?v=tld-9yvX1Dw) | [Point only](https://www.youtube.com/watch?v=FaF-DQgH-HQ&feature=youtu.be) | [Gold and point](https://www.youtube.com/watch?v=PxLzGXmJwzM&feature=youtu.be) | [Whole screen](https://www.youtube.com/watch?v=pRbrS7qmtoQ)

##### Features

* Buying spells
  * Using gold
  * Using skillpoints (can buy/sell skillpoints)
  * Using both gold and skillpoints
* Selling spells
* Showing info
  * About the spellshop, or about your mod, or you can even write a novel so people have something to do while respawning
* Custom icons

##### Usage

* Put the files in their correct folders
* It's not necessary to edit the .swf, but feel free to do so (source is included in "src SpellShopUI" folder)
* Check and edit the files in "scripts/spell_shop_ui/"
* **Check and edit Lua files in "scripts/vscripts/spell_shop_ui.lua"**
  * I'm no Lua coder, so I called the SpellShopUI:InitGameMode(); from within addon_game_mode.lua
  * **The spells don't work as it is (the casting)! You have to precache stuff or do something else within Lua - I don't know, it's up to you.**
    * Check Legends of Dota by Ash47 or something. I'm sorry, I can't help you with that
* Put your custom icons (128 x 128) in "resource/flash3/images/spellicons/", PNG format

###### Events

* Located in custom_events.txt, most are self explanatory
* I didn't list all of them here

```
"spell_shop_ui_toggle_state"
	{
		"player_ID"		"short"
	}
// toggle the _canOpen stat of the shop (if true changes to false, if false changes to true)

"spell_shop_ui_shop_open"
	{
		"player_ID"		"short"
	}
// force the shop open (for example, when entering the trigger area or something. state must allow it)
// "spell_shop_ui_shop_close" is the same but for forcing close

"spell_shop_ui_change_limit"
	{
		"player_ID"		"short"
		"_limit"		"short"
	}
// "_limit" is the number of different spells/abilities a player can own
```

###### Changes
* V1.01
```
added spells_default.txt
  - set default values for spells, other than _ID. then you dont have to write everything in the spells.txt, just the values that you dont want to pull from the spells_default.txt
```

###### Contact

* Please contact me with any requests or bugs. Constructive and uncostructive criticism is welcomed aswell.
```
zed` or zed`` on #dota2mods @ irc.gamesurge.net
reddit.com/u/SelenaGomez_
spellshopui@gmail.com
```

###### Donation

* If you want to donate, I would be more than grateful! 
```
bitcoin: 1M7E87NXXEpVf3vi4FfGqBSp2e5SbgV1jG
```
