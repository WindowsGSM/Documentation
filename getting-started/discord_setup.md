# Discord Setup

## Discord Bot
### Create Bot
<ol>
  <li>Go to <link>https://discord.com/developers/applications</link></li>
  <li>Click on "New Application" in the upper-right</li>
  <li>Give it a name of your choosing and select the tickbox for the ToS</li>
  <li>Click "Create"</li>
  <li>Select "Bot" in the list on the left</li>
  <li>In the section labeled "Privileged Gateway Intents", enable the option for "MESSAGE CONTENT INTENT"<br><b>This will allow the bot to read messages in the Discord server.</b></li>
  <li>Scroll back to the top and under "Token", click on "Reset Token". Copy the token value.</li>
</ol>

### Setup Bot
<ol>
  <li>In WindowsGSM, go to the Discord tab</li>
  <li>Click "Edit" next to "Discord Bot Token", paste in the copied token, and click "Save"</li>
  <li>CLick on the "Invite" button near the top<br><b>This will take you to Discord.</b></li>
  <li>Select the correct server from the list and click continue</li>
  <li>Review and authorize the requested permissions.</li>
</ol>

## Setup Admin Accounts
You will need to explicitly provide which Discord users will be permitted to use the bot commands. Each admin user will need to perform these steps.

### Get User ID from Discord
<ol>
  <li>In Discord, find the user to be added as an admin. This can be done from a post or the members list in a server</li>
  <li>Right-click on the user and select "Copy User ID"</li>
</ol>

### Add Admin User to WindowsGSM
<ol>
  <li>Go to the Discord tab in WindowsGSM</li>
  <li>Click "ADD ADMIN ID" in the upper-right</li>
  <li>Paste in the ID provided from above<br><b>By default, the admin will have permissions to manage all servers. If they should only have permissions for specific servers, continue to the next step. Otherwise, stop here.</b></li>
  <li>Click "EDIT SERVER ID" in the upper-right</li>
  <li>Provide a list of server IDs they should be able to manage using the provided sample format![image](https://github.com/WindowsGSM/Documentation/assets/49689423/2960d96f-72fc-4f69-bbf8-399fd2b421c2)
</li>
</ol>

## Discord Webhooks
These are used to provide notifications for server status changes. Webhooks are setup per server in WindowsGSM. This allows for setting up a webhook per channel in Discord per server in WindowsGSM. This allows for granularity so that notifications for a particular game server are only posted in the relevant Discord channel. All game servers can be setup with a single webhook to have all notifications posted to a single channel in Discord.

### Generate Webhook URL
<ol>
  <li>In Discord, go to the channel where you'd like the alerts to be sent for the game server</li>
  <li>Right-click the channel name and select "Edit Channel"</li>
  <li>Select "Integrations from the left-hand menu</li>
  <li>Click on "Create Webhook"<br><b>If you already have a webhook setup, click on "View Webhooks" and then select "New Webhook" instead</b><br><b>The webhook name will autogenerate</b></li>
  <li>Select the newly created webhook</li>
  <li>Click on "Copy Webhook URL"<br><b>You can optionally rename the webhook as well, but this is not required.</b></li>
</ol>

### Setup Webhook in WindowsGSM
<ol>
  <li>Select the game server from the list in WindowsGSM that you want to setup the webhook for</li>
  <li>In the settings pane (bottom left-hand), click on "Edit" next to "Discord Alert"</li>
  <li>Paste in the webhook URL copied from above and click save</li>
  <li>Turn on the toggle next to "Discord Alert"</li>
  <li>Click on "Test Alert" and you should see a message pop into the Discord channel</li>
</ol>

From here, you can configure some of the alert behaviors. 

#### Set Message
This is a preconfigured, static message that will always been shown when the alert fires. This can be set to mention a user for push notifications/alerts from Discord. To do so, get the user's ID from the section above "Get User ID from Discord" and use it in the text field following the example formatting shown.<br><b>The carrots ARE REQUIRED for @ notifications to work</b>

#### Settings
This allows you to select from a list of events that will trigger an alert through the webhook.
