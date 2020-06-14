---
description: A global server config file for WindowsGSM
---

# WindowsGSM.cfg

WindowsGSM.cfg will be auto-created after the game server installed successfully. This config file stores the most common parameters like _IP_, _port_, _map_, _maxplayer,_ etc. These values will be loaded as server start parameters. If you would like to add custom start parameters, see \#additional-parameters below. 

## Basic server settings

<table>
  <thead>
    <tr>
      <th style="text-align:left">Key</th>
      <th style="text-align:left">Notes</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">servergame</td>
      <td style="text-align:left">Do <b>NOT</b> edit this field</td>
    </tr>
    <tr>
      <td style="text-align:left">servername</td>
      <td style="text-align:left">
        <p>Game server name - Set the hostname of the game server here.</p>
        <p><b><code>&#x26A0;&#xFE0F; Some servers use their own server config to set the hostname</code></b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">serverip</td>
      <td style="text-align:left">
        <p>Game server IP - Set the start IP of the game server here.</p>
        <p><b><code>&#x26A0;&#xFE0F; Some servers use their own server config to set the IP</code></b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">serverport</td>
      <td style="text-align:left">
        <p>Game server Port - Set the start port of the game server here.</p>
        <p><b><code>&#x26A0;&#xFE0F; Some servers use their own server config to set the Port</code></b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">serverqueryport</td>
      <td style="text-align:left">
        <p>Game server Query Port - Set the query port of the game server here.</p>
        <p><b><code>&#x26A0;&#xFE0F; Some servers use their own server config to set the Query Port</code></b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">servermap</td>
      <td style="text-align:left">Game server map - Set the startup map of the game server here.</td>
    </tr>
    <tr>
      <td style="text-align:left">servermaxplayer</td>
      <td style="text-align:left">Game server maxplayer - Set the max player of the game server here.</td>
    </tr>
    <tr>
      <td style="text-align:left">servergslt</td>
      <td style="text-align:left">Game server GSLT token - Set the GSLT token of the game server</td>
    </tr>
    <tr>
      <td style="text-align:left">serverparam</td>
      <td style="text-align:left">Additional parameters - Set the addition start param here</td>
    </tr>
  </tbody>
</table>

## CPU Priority and Affinity

| Key | Notes |
| :--- | :--- |
| cpupriority | CPU Priority - Set the default priority for game process |
| cpuaffinity | CPU Affinity - Set the default affinity for game process |

## Automation

| Key | Notes |
| :--- | :--- |
| autorestart |  |
| autostart |  |
| autoupdate |  |
| updateonstart |  |
| backuponstart |  |
| restartcrontab |  |
| crontabformat |  |

## Discord Webhook Alert

| Key | Notes |
| :--- | :--- |
| discordalert |  |
| discordmessage |  |
| discordwebhook |  |
| autostartalert |  |
| autorestartalert |  |
| autoupdatealert |  |
| restartcrontabalert |  |
| crashalert |  |

## Miscellaneous

| Key | Notes |
| :--- | :--- |
| embedconsole |  |

## Default WindowsGSM.cfg format

Sample of [Minecraft: Java Edition Server](supported-game-servers/minecraft-java-edition.md)'s WindowsGSM.cfg

```csharp
servergame="Minecraft: Java Edition Server"
servername="WindowsGSM - Server #1"
serverip="10.0.0.2"
serverport="25565"
serverqueryport="25565"
servermap="world"
servermaxplayer="20"
servergslt=""
serverparam="-Xmx1024M -Xms1024M"

cpupriority="2"
cpuaffinity="11111111"

autorestart="0"
autostart="0"
autoupdate="0"
updateonstart="0"
backuponstart="0"

discordalert="0"
discordmessage=""
discordwebhook=""

restartcrontab="0"
crontabformat="0 6 * * *"

embedconsole="0"

autostartalert="1"
autorestartalert="1"
autoupdatealert="1"
restartcrontabalert="1"
crashalert="1"

```

