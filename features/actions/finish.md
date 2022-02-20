# Finish action

The action that sets off the fireworks

### Example config

[comment]: <> (armasm, d, ini, kotlin, makefile, perl, python, r, swift, x86asm)

```kotlin
title = "Eggs Category"
hidePlayerData = false
category = "category2"

finishAction {
  sound = "UI_TOAST_CHALLENGE_COMPLETE"
  message {
    title = "&aFinish!"
    subtitle = "&eyou have found them all :)"
    fadeIn = 10
    fadeOut = 10
    stay = 50
  }
}
`````