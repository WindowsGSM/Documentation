# Discord Bot Setup and Configuration

## Step 1: Create a new Discord Application
Follow the ![Generating your Discord Bot Token](https://www.writebots.com/discord-bot-token/#Generating_Your_Token_StepbyStep) guide to create a new Discord application.
You will be required to login to the Discord Developer panel.
## Step 2: Get your token
The ![next steps in the same guide](https://www.writebots.com/discord-bot-token/#4_Retrieve_Your_Token) will show you how to generate and access your token. Copy this and keep it handy for the next step...
## Step 3: Configure WindowsGSM
* Click on the Discord Bot icon in the side panel of WindowsGSM
* Click on "EDIT" above the "Discord Bot Token" line, paste in your copied Discord Token, and click "SAVE" to apply.
* Edit the "Bot Prefix" line with whatever you'd like (default is usually "!"). You will use this prefix before any commands.
* Specify which Discord Channel you'd like for the bot in "Dashboard Channel ID". This is where the Discord Bot will submit status reports.
## Step 4: Assign Admins
Follow ![this guide](https://support.discord.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-) to enable "Developer Mode" in Discord and obtain the full "User ID" for any admins you would like to control the Discord Bot.
> The User ID will be a numeric value like: ```20608908013862xxxx```

In WindowsGSM, click on "ADD ADMIN ID" and paste in the User ID.

> Server ID will default to "0" which allows admins to control any server. Click on "EDIT SERVER ID" and adjust this value if necessary.

## Step 5: Invite and Test
The final step is inviting the bot to your Discord server. Simply click the "INVITE" button and your bot should join.
Feel free to attempt commands, being sure to use the prefix you defined in *step 3*.
