# TTT Traitor Weapon

This addon includes a basic TTT Weapon that can be bought by traitors from the equipment store.

See the [Official Guide](http://ttt.badking.net/custom-weapon-guide) for a more detailed explanation of the different weapon properties.

<br>

## Files

The weapon code can be found in `lua/weapons/weapon_ttt_sample_ak47.lua`

The file `addon.json` includes information used when uploading the addon to the workshop.

<br>
<br>

## Tips

<br>

### Detective weapons
To allow detectives to buy this weapon, you will need to change the property:<br>
`SWEP.CanBuy`<br>
in `lua/weapons/weapon_ttt_sample_ak47.lua`.

* **Traitor-only equipment**
    * `SWEP.CanBuy = { ROLE_TRAITOR }`
* **Detective-only equipment**
    * `SWEP.CanBuy = { ROLE_DETECTIVE }`
* **Traitor & Detective equipment**
    * `SWEP.CanBuy = { ROLE_TRAITOR, ROLE_DETECTIVE }`

<br>

### Making a custom icon
[Follow this guide](https://github.com/BadgerCode/TTT-Developer-Resources/tree/master/weapons/icons#custom-weapon-icons) to make a custom icon for your weapon.


<br>
<br>


## Testing
* [Copy the addon to your Garry's Mod folder](https://github.com/BadgerCode/GMod-Addon-Samples#usage)
* Start up Garry's Mod.
    * If you already had Garry's Mod open before creating your addon folder:
        * [Open the developer console](https://steamcommunity.com/sharedfiles/filedetails/?id=627640216)
        * Type `reload_legacy_addons` and press enter
* Play TTT
    * If you are already playing TTT singleplayer
        * [Open the developer console](https://steamcommunity.com/sharedfiles/filedetails/?id=627640216)
        * Type `reload` and press enter
    * Click Start New Game
    * Set the gamemode to TTT
    * Select any map (e.g. `gm_construct`)
    * Click Start Game
* Allow yourself to spawn
    * [Open the developer console](https://steamcommunity.com/sharedfiles/filedetails/?id=627640216)
    * Type `ttt_debug_preventwin 1` and press enter
    * Type `ttt_minimum_players 1` and press enter
* Spawn the weapon
    * [Open the developer console](https://steamcommunity.com/sharedfiles/filedetails/?id=627640216)
    * Type `give weapon_ttt_sample_ak47` and press enter
        * _weapon_ttt_sample_ak47_ is the name of the weapon file

