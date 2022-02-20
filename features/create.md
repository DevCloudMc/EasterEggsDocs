# Create EasterEggs
Once you've created the group u can start editing it and adding new easter eggs by
typing `/ee edit <category_name>`.

To add a new easter egg just click RMB on any block/armorstand/painting/frame/~~npc~~.
A new easter eggs with unique ID will be created.

To remove any easter egg just click LBM on it while editing.

## Adding actions to easter eggs
Easter eggs actions are adding in edit mode. To add an action just type
`/ee action add <easter_egg_id> <action_name> <action_data>`

`<action_name>` value is the name of one of the following action types:

| Param      | Description                                  |
|------------|----------------------------------------------|
| `message`  | Chat/actiobar/title message.                 |
| `commands` | Running commands by the player or server     |
| `sound`    | Playing sound for the player                 |
| `money`    | Gives any amount of money                    |
| `firework` | Launching a firework                         |

Those actions are in the json format. Data depends on the variables of
specified action.