asset_get
==========


Returns the unique index (real) for any built-in game asset - including sounds, objects, and sprites. Can be used, for example, to assign a specific sound effect to a character attack.

*   [Available SFX list](/workshop/sfx-list/)
*   [Available Object List](https://www.rivalsofaether.com/workshop/available-objects/)

To get the index of a custom (loaded with your character) asset, use

`sprite_get( sprite )` [Reference](/code/roa/sprite_get)

`sound_get( sound )` [Reference](/code/roa/sound_get) functions instead.

<span class='argdesc'>

| Argument| Type    | Description                                                                  |
|---------|---------|------------------------------------------------------------------------------|
|asset    |string   | The name of the game asset to get the index of Example, called from bair.gml:|


</span>

```gml
// sets the sound effect assigned to the 3rd bair window:

set_window_value( AT_BAIR, 3, AG_WINDOW_SFX, asset_get( "sfx_swipe_medium1" ));
```
