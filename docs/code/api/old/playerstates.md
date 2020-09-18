### States

Use these values when changing states with set_state( state )  Reference→

To check the state of a character, use the state variable.

PS_WALK
PS_WALK_TURN
PS_DASH_START
PS_DASH
PS_DASH_STOP
PS_DASH_TURN
PS_WAVELAND

PS_AIR_DODGE
PS_PARRY_START
can transition into rolls or parry, depending on direction held
PS_PARRY
PS_ROLL_BACKWARD
PS_ROLL_FORWARD
PS_TECH_GROUND
PS_TECH_BACKWARD
PS_TECH_FORWARD
PS_WALL_TECH

PS_WRAPPED
PS_FROZEN
PS_IDLE
PS_IDLE_AIR
PS_CROUCH
PS_JUMPSQUAT
PS_FIRST_JUMP
PS_DOUBLE_JUMP
PS_WALL_JUMP
PS_LAND

PS_ATTACK_AIR
PS_ATTACK_GROUND
PS_LANDING_LAG

PS_HITSTUN
PS_HITSTUN_LAND
PS_TUMBLE
PS_PRATFALL
PS_PRATLAND

PS_SPAWN
PS_RESPAWN
PS_DEAD


### State Categories

These values are set automatically depending on the state and should not be manually changed. To check a character’s state category, use the `state_cat` variable.


```bash
SC_HITSTUN ▼
	PS_HITSTUN
	PS_HITSTUN_LAND
	PS_WRAPPED
	PS_FROZEN
```
SC_AIR_NEUTRAL ▼
PS_IDLE_AIR
PS_FIRST_JUMP
PS_DOUBLE_JUMP
PS_TUMBLE

SC_AIR_COMMITTED ▼
PS_WALL_JUMP
PS_ATTACK_AIR
PS_PRATFALL
PS_AIR_DODGE
PS_WALL_TECH
PS_RESPAWN
PS_DEAD
SC_GROUND_NEUTRAL ▼
PS_IDLE
PS_CROUCH
PS_WALK

SC_GROUND_COMMITTED ▼
PS_LAND
PS_SPAWN
PS_PRATLAND
PS_LANDING_LAG
PS_WALK_TURN
PS_ATTACK_GROUND
PS_WAVELAND
PS_DASH_START
PS_DASH
PS_DASH_TURN
PS_DASH_STOP
PS_PARRY_START
PS_PARRY
PS_TECH_GROUND
PS_TECH_BACKWARD
PS_TECH_FORWARD
PS_ROLL_BACKWARD
PS_ROLL_FORWARD
PS_JUMPSQUAT