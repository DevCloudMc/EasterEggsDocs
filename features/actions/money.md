# Money

Action to give money to a player

### Structure
| Param       | Description                                              | Value type       |
|-------------|----------------------------------------------------------|------------------|
| `money`     | The amount of money to be handed out                     | Float or Integer |

### Examples

At the moment, this action can only be added via config.

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
    money = 100
  }
}
```