# Message

The action that sets off the fireworks

### Structure

| Param     | Description                                                 | Default | Value type     |
|-----------|-------------------------------------------------------------|---------|----------------|
| `power`   | The distance the fireworks will fly. power = 0 ~ 4-5 blocks | 0       |     Integer    |
| `effects` | Effects list                                                | Random  | List of String |

Colors for effects must be set in HEX. The number of effects is unlimited.

### Examples

At the moment, this action can only be added via config.

### Example config

[comment]: <> (armasm, d, ini, kotlin, makefile, perl, python, r, swift, x86asm)

```kotlin
title = "Eggs Category"
hidePlayerData = false
category = "category2"

"0" {
  location = "world, 0.0, 0.0, 0.0"
  type = "BLOCK"
  id = 0;
  actions {
    firework {
      power = 1
      effects: [
        {
          type = BALL
          trail = false
          colors: [
            "FF00FF",
            "FF00FF",
            "F000F0"
          ]
          fadeColors: [
            "000000",
            "FF0000"
          ]
        }
      ]
    }
}
```