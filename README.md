Configurable logging of chat, commands, connections, and more

**Logger** provides configurable logging for chat messages, chat commands, console commands, and player respawns. Each type of logging can be enabled/disabled via the configuration file. Logs are stored under the oxide/logs folder.

## Configuration
You can configure the settings in the Logger.json file under the oxide/config directory.
```json
{
  "Command Exclusions": [
    "help",
    "version",
    "chat.say",
    "craft.add",
    "craft.canceltask",
    "global.kill",
    "global.respawn",
    "global.respawn_sleepingbag",
    "global.status",
    "global.wakeup",
    "inventory.endloot",
    "inventory.unlockblueprint"
  ],
  "Log Chat (true/false)": false,
  "Log Commands (true/false)": true,
  "Log Connections (true/false)": true,
  "Log Disconnections (true/false)": true,
  "Log Respawns (true/false)": false,
  "Log to Console (true/false)": true
}
```

## Localization
The default messages are located in the Logger.en.json under the oxide/lang directory. Language files are also available for French, German, Russian, and Spanish. To add support for another language, create a new language folder (ex. de for German), copy the default language file to the new folder, and then customize the messages.
```json
{
  "Command": "{0} ({1}) ran command: {2} {3}",
  "Connected": "{0} ({1}) connected from {2}",
  "Disconnected": "{0} ({1}) disconnected",
  "Respawned": "{0} ({1}) respawned at {2}"
}
```
