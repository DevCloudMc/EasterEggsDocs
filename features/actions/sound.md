# Sound

Action that plays the sound

### Structure
| Param      | Description                                                                                                                 | Default         | Value type |
|------------|-----------------------------------------------------------------------------------------------------------------------------|-----------------|------------|
| `type`     | Sound name. Here you can find all of them:  [Sound types](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/Sound.html)   |                 |   String   |
| `location` | Sound format playback location: `"world,x,y,z"`                                                                             | Player location |   String   |
| `pitch`    | The pitch of the volume                                                                                                     | 1.0             |    Float   |
| `volume`   | How loud the sound                                                                                                          | 1.0             |    Float   |

### Examples
Example json format:  
`{type="SOUND_TYPE_NAME" location="world,0,0,0"}`

Command to add an action for an easter egg:  
`/ee action add <egg_id> sound {type="ENTITY_PLAYER_LEVELUP" location="world,0,60,-133"}`

### Example config

[comment]: <> (armasm, d, ini, kotlin, makefile, perl, python, r, swift, x86asm)

```kotlin
title = "Eggs Category"
hidePlayerData = false
category = "category2"

"0" {
  location = "world, 0.0, 1.0, 0.0"
  type = "BLOCK"
  id = 0
    actions {
        sound {
            type: "ENTITY_PLAYER_LEVELUP"
            location: "world, -99.47, 4.0, -380.93"
        }
    }
}
```