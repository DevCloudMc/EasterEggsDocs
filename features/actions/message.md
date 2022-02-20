# Message

Action to display text on the player's screen. This can be either a regular chat message to the player or an action bar & title with subtitle

### Structure
| Param       | Description                                                     | Default value | Value type |
|-------------|-----------------------------------------------------------------|---------------|------------|
| `messages`  | List of messages displaying in the chat. That's how it looks in |               |   String   |
| `title`     | Title message                                                   |               |   String   |
| `subTitle`  | Subtitle message                                                |               |   String   |
| `actionbar` | Actionbar message                                               |               |   String   |
| `fadeIn`    | Title fade in period in ticks _(1 second = 20 ticks)_           | 10 (in ticks) |   Integer  |
| `fadeOut`   | Title fade out period in ticks                                  | 10 (in ticks) |   Integer  |
| `stay`      | Delay period before fade out starts in ticks                    | 30 (in ticks) |   Integer  |

`fadeIn`, `fadeOut`, `stay` parameters only affect the following `actionBar`, `title` or `subTitle` parameters
### Examples
Example json format:  
`{messages:["Message 1", "Message 2"]}`

For example, if u want to display something in actionbar, you should type:  
`/ee action add <egg_id> message {actionbar:"Hello, world!"}`  
or  
`/ee action add <egg_id> message {messages=["&eFirst", "&cSecond"]}`

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
    message {
      messages: [
        "Hello world!",
        "..."
      ]
      title = "Title text"
      subTitle = "subtitle text"
      actionBar = "Actionbar text"
      fadeIn = 10
      stay = 40
      fadeOut = 10
    }
  }
}
```