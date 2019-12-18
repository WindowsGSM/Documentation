# Configuration

## WindowsGSM.cfg

WindowsGSM.cfg will be auto-created after the game server installed successfully. This config file's values will be loaded as server start parameters. 

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

| Key | Default value | Usage |
| :--- | :--- | :--- |
| `servergame` | _&lt;auto-generate&gt;_ | Define the game type \(**DO NOT EDIT**\) |
| `servername` | _&lt;auto-generate&gt;_ | Define the display name of the server |
| `serverip` | _&lt;local-IP&gt;_ | server IP |
| `serverport` | _&lt;auto-generate&gt;_ | server Port |
| `servermap` | _&lt;auto-generate&gt;_ | server Map |
| `servermaxplayer` | _&lt;auto-generate&gt;_ | server Max Players |
| `servergslt` |  | server GSLT |
| `serverparam` | _&lt;auto-generate&gt;_ | server additional start-up parameter |
| `autorestart` | `1` | `1`= Enable / `0` = Disable auto restart function |
| `updateonstart` | `0` | `1` = Enable / `0` = Disable update on start function  |
| `discordalert` | `0` | `1` = Enable / `0` = Disable discord alert function |
| `discordwebhook` |  | Discord Webhook URL |



