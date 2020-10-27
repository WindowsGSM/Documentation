# Discord Bot Setup and Configuration
![Screenshot DiscordBot](https://windowsgsm.com/assets/images/WindowsGSM-DiscordBot-v1.18.0.png)

## Step 1: Create a new Discord Application
Follow the [Generating your Discord Bot Token](https://www.writebots.com/discord-bot-token/#Generating_Your_Token_StepbyStep) guide to create a new Discord application.
You will be required to login to the Discord Developer panel.
## Step 2: Get your token
The [next steps in the same guide](https://www.writebots.com/discord-bot-token/#4_Retrieve_Your_Token) will show you how to generate and access your token. Copy this and keep it handy for the next step...
## Step 3: Configure WindowsGSM
* Click on the Discord Bot icon in the side panel of WindowsGSM
* Click on "EDIT" above the "Discord Bot Token" line, paste in your copied Discord Token, and click "SAVE" to apply.
* Edit the "Bot Prefix" line with whatever you'd like (default is usually "!"). You will use this prefix before any commands.
## Step 4: Assign Admins and Channel
Follow [this guide](https://support.discord.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-) to enable "Developer Mode" in Discord. Developer mode allows you to obtain the full numerical ID number for users/channels/servers/etc.
With developer mode enabled, simply right click your user and click on "Copy ID"
> The User ID will be a numeric value like: ```20608908013862xxxx```

In WindowsGSM, click on "ADD ADMIN ID" and paste in the User ID.

> Server ID will default to "0" which allows admins to control any server. Click on "EDIT SERVER ID" and adjust this value if necessary.

Finally, right click on the channel that you'd like the bot in and copy that ID. This will be put in "Dashboard Channel ID" line in WindowsGSM to designate which channel the bot will submit status reports, etc.

## Step 5: Invite and Test
The final step is inviting the bot to your Discord server. 

Hit the "Enable" toggle switch and make sure the log shows that the Discord bot started properly. Then, simply click the "INVITE" button and your bot should join.

Feel free to attempt commands, being sure to use the prefix you defined in *step 3* and in a channel that the bot has access to.
