<style>
	code, pre {
		font-family: "Fira Code", "Consolas", monospace;
	}
	em {
	 color: silver;
	}
</style>

Configuration File
==================

All workshop items (characters, stages, and buddies) need a `config.ini` file to indicate which type of workshop item it is. This file also provides useful information about the workshop item. 

> If this is configured incorrectly your character cannot be uploaded.  
> **Any `key` wrapped in brackets `[ ]` indicates an optional value**

### Config.ini


|Key                  |Description                                    |Notes                                    |Value Examples                                                    									|
|:--------------------|:----------------------------------------------|:--------------------------------------- |:--------------------------------------------------------------------------------------------------|
|`type`               |_sets the type of your workshop item_          | *indicates a character, buddy or stage* |`0`(**character**), `1` (**buddy**), `2` **stage**                									|
|`name`               |_the name of the workshop item_                | 								        |**_Sandbert_**                                                    									|
|`description`        |_workshop item description for Steam_          | 								        |**_A broken sand bag_**                                           									|
|`major version`      |_primary digit in version_;                    |*manually upadated in the config*        |**1**.3 (_the `1` is the major version_);                         									|
|`minor version`      |_secondary digit in version_;                  |*auto updated when uploading*            | 1.**3** (_the `3` is the minor version_)                         									|
|`author`             |_creator of the workshop item_                 |*overridden if Steam nick is used*       | **iivii**                                                        									|
|`[url]`              |_link to already uploaded item_                |*use only the `ID` part of link*         |`1875062006`													   									|
|`[finished]`         |_indicates a completed workshop item_          |*item is tagged as completed on Steam*   | `1` (**DONE**); `0` (**WIP**)                                    									|
|`plural`             |_grammar for team based workshop items_        |*pluralizes __win__ to __wins__*         | `1` 																								|
|`info1 info2 info3`  |_information displayed at character select_    |*each of these is a __separate key__!*   |																									|
| `bg color`          |_background color in character select_         |*usually matches the character’s element*|`red`/`fire`, `pink`/`air`, `blue`/`water`, `green`/`earth`, `none`/`aether`/`purple`, **custom**	|
|`[bg red]`           |_red component of **custom** bg color_         |*only valid if `bg color` is `custom`*   |`0`-`255`																							|
|`[bg green]`         |_green component of **custom** bg color_       |*only valid if `bg color` is `custom`*   |`0`-`255`																							|
|`[bg blue]`          |_blue component of **custom** bg color_        |*only valid if `bg color` is `custom`*   |`0`-`255`																							|

