sprite_get
==========


Returns the unique index(<span class="code-line"><span class="type">real</span></span>) of the sprite asset loaded from the <span class="code-line">/sprites</span> folder.

| Argument                                                         | Type                                                             | Description                                    |
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------- |
|`sprite`                                                          | **string**                                                       | _The name of the game asset to get the index of_ |


Examples
---------

Called from <span class="code-line">animation.gml</span>:

```gml
if (state == PS_WALK) { 
	sprite_index = sprite_get( "dash" ); 
}
```
