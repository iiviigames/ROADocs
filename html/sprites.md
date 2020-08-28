A sprite should be a strip of animation frames, sequenced one after
another from the left to the right. All frames should have the same
dimensions. Sprites should be named in the following pattern:
<span class="code-line"><span class="type">\[name\]</span>\_strip<span class="type">\[frames\]</span>.png</span>.
For example: <span class="code-line">walk\_strip8.png</span>, telling
the parser the animation has 8 frames.

To convert a gif into a sprite sheet, you can either use Game Maker to
import and export it as a .png or use an online converter like [this
one](https://ezgif.com/gif-to-sprite) (use the "Stack Horizontally"
option to make sure everything is on a single row).

<div class="important">

If you want the sprite to replace one of the existing character states
without any scripting, you should [name it
accordingly](https://www.rivalsofaether.com/workshop/animation-names/).

</div>

Hurtbox sprites for non-attack states
(<span class="code-line">\_hurtbox</span>,
<span class="code-line">\_crouchbox</span>,
<span class="code-line">\_hurtbox\_air</span>,
<span class="code-line">\_hitstun\_hurtbox</span>) use rectangular
collision. Hurtbox sprites for attacks
(<span class="code-line">\_hurt</span> sprites) use precise collision
instead.

The origin for all sprites is set to top left (0, 0) by default. To help
place origins correctly, use the [Rivals Workshop
Helper](https://github.com/dfornace/workshophelper).

You can directly reference any custom sprite by calling
<span class="code-line"><span class="function">sprite\_get(</span>
name<span class="type">:string</span>
<span class="function">)</span></span> in
<span class="code-line">animation.gml</span>. For example, forcing walk
animation to use the dash sprite instead:

`if (state == PS_WALK) { sprite_index = sprite_get( "dash" ); }`

([reference](https://www.rivalsofaether.com/workshop/player-states) on
available player states).

You can also change offset and bounding boxes for your sprites in
<span class="code-line">load.gml</span>. For example:

`// changing offset of the jump sprite to [94, 138]:
sprite_change_offset( "jump", 94, 138 ); // making it precise:
sprite_change_collision_mask( "jump", true, 0, 0, 0, 0, 0, 0 );`

### Hit Particles

Hit Particles have a couple differences to how normal sprites work;
visit the [page for Hit
Particles](https://rivalsofaether.com/workshop/hit-particles/) to learn
more about how to change those for your character.
