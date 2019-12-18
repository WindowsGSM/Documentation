# Configuration

## WindowsGSM.cfg

WindowsGSM.cfg will be auto-created after the game server installed successfully. This config file stores the most common parameters like _IP_, _port_, _map_, _maxplayer,_ etc. These values will be loaded as server start parameters. If you would like to add custom start parameters, see \#additional-parameters below. 

Sample of [Minecraft: Java Edition Server](../game-servers/supported-game-servers/minecraft-java-edition.md)'s WindowsGSM.cfg

```text
servergame="Minecraft: Java Edition Server"
servername="WindowsGSM - Server #1"
serverip="10.0.0.2"
serverport="25565"
servermap="world"
servermaxplayer="20"
servergslt=""
serverparam="-Xmx1024M -Xms1024M"

autorestart="1"
updateonstart="0"

discordalert="0"
discordwebhook=""

```

### Additional Parameters

If you would like to add custom start parameters, you can edit `serverparam` variable. The values in `serverparam` will be added into the start parameter.

#### Example

`serverparam="-tickrate 64 -usercon"`

{% hint style="info" %}
More parameters: [https://developer.valvesoftware.com/wiki/Command\_Line\_Options](https://developer.valvesoftware.com/wiki/Command_Line_Options#Command-line_parameters_3)
{% endhint %}

