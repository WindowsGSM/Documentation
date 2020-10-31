# Discord Bot Setup and Configuration
![Screenshot DiscordBot](https://windowsgsm.com/assets/images/WindowsGSM-DiscordBot-v1.18.0.png)

## Step 1: Create a new Discord Application
The first thing we need to do is create a new Discord Application from the [Discord Developer Portal](https://discordapp.com/developers/applications/me).

Click [here](https://discordapp.com/developers/applications/me) to login, and click on "New Application" at the top-right.
> There are several guides available [here](https://www.writebots.com/discord-bot-token/#Generating_Your_Token_StepbyStep) and [here](https://github.com/reactiflux/discord-irc/wiki/Creating-a-discord-bot-&-getting-a-token) to help create an application and generate a token.

## Step 2: Get your token
The next step is generating your bot token.

* After creating your new application, click on the puzzle piece icon titled "Bot" on the left sidebar. 
* Click on "Add Bot" and accept. You will see a link to display your token, and a button under it to copy it to your clipboard.

All you need here is your bot token. Copy it and come back here for the next steps. Ignore any further steps in the linked guides - they aren't necessary.
> The guides linked above cover the steps to retrieve your bot token. Click [here](https://www.writebots.com/discord-bot-token/#Generating_Your_Token_StepbyStep) for the direct link.

## Step 3: Configure WindowsGSM
Back in WindowsGSM:
* Click on the Discord Bot icon in the side panel of WindowsGSM
* Click on "EDIT" above the "Discord Bot Token" line, paste in your copied Discord Token, and click "SAVE" to apply.
* Edit the "Bot Prefix" line with whatever you'd like (default is usually "!"). (you will use this prefix in Discord chat before any commands, such as ```!wgsm check```

## Step 4: Assign Admins and Channel
We need to enable Developer Mode in Discord next.

Developer mode allows you to obtain the full numerical ID number for users/channels/servers/etc.

Follow [this guide](https://support.discord.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-) to enable "Developer Mode" in Discord.

* With developer mode enabled, simply right click your user and click on "Copy ID"
> The User ID will be a numeric value like: ```20608908013862xxxx```

* In WindowsGSM, click on "ADD ADMIN ID" and paste in the User ID.

> Server ID will default to "0" which allows admins to control any server. Click on "EDIT SERVER ID" and adjust this value if necessary.

* Finally, right click on the channel that you'd like the bot in and copy that ID. This will be put in "Dashboard Channel ID" line in WindowsGSM to designate which channel the bot will submit status reports, etc.

## Step 5: Invite and Test
The final step is inviting the bot to your Discord server. 

* Hit the "Enable" toggle switch and make sure the log shows that the Discord bot started properly.
* Then, simply click the "INVITE" button.

If everything works correctly, your browser should open to a page requesting permission for your bot to join your Discord. Click through these without changes, and you should see the bot has joined your Discord server.

Feel free to attempt commands, being sure to use the prefix you defined in *step 3* and in a channel that the bot has access to.
