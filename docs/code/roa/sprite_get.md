### sprite_get


Returns the unique index(<span class="code-line"><span class="type">real</span></span>) of the sprite asset loaded from the <span class="code-line">/sprites</span> folder.

| Argument                                                         | Type                                                             | Description                                    |
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------- |
| <span class="code-line"><span class="macro">sprite</span></span> | <span class="code-line"><span class="type">:string</span></span> | The name of the game asset to get the index of |


Example, called from <span class="code-line">animation.gml</span>:

```gml
if (state == PS_WALK) { 
	sprite_index = sprite_get( "dash" ); 
}
```
