---
description: A global server config file for WindowsGSM
---

# WindowsGSM.cfg

WindowsGSM.cfg will be auto-created after the game server installed successfully. This config file stores the most common parameters like _IP_, _port_, _map_, _maxplayer,_ etc. These values will be loaded as server start parameters. If you would like to add custom start parameters, see \#additional-parameters below. 

Sample of [Minecraft: Java Edition Server](supported-game-servers/minecraft-java-edition.md)'s WindowsGSM.cfg

```csharp
servergame="Minecraft: Java Edition Server"
servername="WindowsGSM - Server #1"
serverip="10.0.0.2"
serverport="25565"
servermap="world"
servermaxplayer="20"
servergslt=""
serverparam="-Xmx1024M -Xms1024M"

autorestart="0"
autostart="0"
autoupdate="0"
updateonstart="0"

discordalert="0"
discordwebhook=""

```

## `servergame` - Game Server Type

Do _**NOT**_ edit this field, the field is for WindowsGSM to recognize the game server type.

## `servername` - Game Server Name

You can set the hostname of the game server here.

{% hint style="warning" %}
Some server use their own server config to set the hostname
{% endhint %}

## `serverip` - Game Server IP

You can set the IP of the game server here.

{% hint style="warning" %}
Some server use their own server config to set the IP
{% endhint %}

## `serverport` - Game Server Port

You can set the gameport of the game server here.

{% hint style="warning" %}
Some server use their own server config to set the port
{% endhint %}

## `servermap` - Game Server Map

You can set the startup map of the game server here.

## `servermaxplayer` - Game Server Maxplayer

You can set the max player of the game server here.

## `servergslt` - Game Server GSLT

You can set the GSLT of the source game server here.

## `serverparam` - Additional Parameters

If you would like to add custom start parameters, you can edit `serverparam` variable. The values in `serverparam` will be added into the start parameter.

#### Example

`serverparam="-tickrate 64 -usercon"`

{% hint style="info" %}
More parameters: [https://developer.valvesoftware.com/wiki/Command\_Line\_Options](https://developer.valvesoftware.com/wiki/Command_Line_Options#Command-line_parameters_3)
{% endhint %}



