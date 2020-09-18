## set_state


?>Changes the character’s [state](code/api/playerstates)  
For attack states use `set_attack` [Reference→](/workshop/set_attack)



|Argument|Type|Description
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------- |
|<span class="code-line"><span class="macro">state</span></span>|<span class="code-line"><span class="type">:real</span></span>|The [state](code/api/playerstates) to set|


Examples
----------


This could be used if called from the `attack_update.gml` script:

```gml
// this attack cancels into pratfall when you press the dodge button:
if (window == 3 && shield_pressed){
	set_state( PS_PRATFALL );
}
```
