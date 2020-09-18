States
=============

?> Use these values when changing states with <span class="code-line"><span class="function">set_state</span>( state )</span> [Reference&#26;](code/roa/set_state)


To check the state of a character, use the <span class="code-line">state</span> variable.



#### Motion

```gml
PS_WALK
PS_WALK_TURN 
PS_DASH_START 
PS_DASH 
PS_DASH_STOP 
PS_DASH_TURN
PS_WAVELAND
```


#### Dodge and Parry

```gml
PS_AIR_DODGE 

//can transition into rolls or parry,depending on direction held 
PS_PARRY_START 

PS_PARRY 
PS_ROLL_BACKWARD 
PS_ROLL_FORWARD
PS_TECH_GROUND
PS_TECH_BACKWARD
PS_TECH_FORWARD 
PS_WALL_TECH 
```


#### Entrapped

```gml
PS_WRAPPED 
PS_FROZEN
```


#### Actions

```gml
PS_IDLE
PS_IDLE_AIR
PS_CROUCH
PS_JUMPSQUAT
PS_FIRST_JUMP
PS_DOUBLE_JUMP
PS_WALL_JUMP 
PS_LAND
```


#### Attacks

```gml
PS_ATTACK_AIR 
PS_ATTACK_GROUND 
PS_LANDING_LAG
```


#### Damage and Clumsiness

```gml

PS_HITSTUN 
PS_HITSTUN_LAND 
PS_TUMBLE 
PS_PRATFALL 
PS_PRATLAND

``` 

#### Transitions


```
PS_SPAWN 
PS_RESPAWN 
PS_DEAD
```


### State Categories

These values are set automatically depending on the state and should not
be manually changed. To check a character's state category, use the
<span class="code-line">state\_cat</span> variable.


<!-- `SC_HITSTUN  PS_HITSTUN PS_HITSTUN_LAND PS_WRAPPED PS_FROZEN`  
`SC_AIR_NEUTRAL  PS_IDLE_AIR PS_FIRST_JUMP PS_DOUBLE_JUMP PS_TUMBLE`  
`SC_AIR_COMMITTED  PS_WALL_JUMP PS_ATTACK_AIR PS_PRATFALL PS_AIR_DODGE
PS_WALL_TECH PS_RESPAWN PS_DEAD` -->


<span class="macro">SC\_GROUND\_COMMITTED &#31;  
<span class="tab"></span>PS\_LAND  
<span class="tab"></span>PS\_SPAWN  
<span class="tab"></span>PS\_PRATLAND  
<span class="tab"></span>PS\_LANDING\_LAG  
<span class="tab"></span>PS\_WALK\_TURN  
<span class="tab"></span>PS\_ATTACK\_GROUND  
<span class="tab"></span>PS\_WAVELAND  
<span class="tab"></span>PS\_DASH\_START  
<span class="tab"></span>PS\_DASH  
<span class="tab"></span>PS\_DASH\_TURN  
<span class="tab"></span>PS\_DASH\_STOP  
<span class="tab"></span>PS\_PARRY\_START  
<span class="tab"></span>PS\_PARRY  
<span class="tab"></span>PS\_TECH\_GROUND  
<span class="tab"></span>PS\_TECH\_BACKWARD  
<span class="tab"></span>PS\_TECH\_FORWARD  
<span class="tab"></span>PS\_ROLL\_BACKWARD  
<span class="tab"></span>PS\_ROLL\_FORWARD  
<span class="tab"></span>PS\_JUMPSQUAT </span>


