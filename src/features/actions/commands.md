# Commands

Action to execute commands on behalf of the player or console

### Structure
| Param       | Description                                               | Value type     |
|-------------|-----------------------------------------------------------|----------------|
| `player`    | Commands list. Specifies whether run a command by console | List of String |
| `console`   | Commands list. Specifies whether run a command by player  | List of String |
### Examples
Example json format:  
`{console:["Command 1", "Command 2"]}`

Example command to add action:  
`/ee action add <egg_id> commands {player=["home", "say Hello"] console=["broadcast Hi!"]}`

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
    commands {
      player = [
        "home",
        "money"
      ]
      console = "say hello!"
    }
  }
}
```