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

### Setup Admin Accounts
You will need to explicitly provide which Discord users will be permitted to use the bot commands. Each admin user will need to perform these steps.

#### Get User ID from Discord
<ol>
  <li>In Discord, go to "Settings"</li>
  <li>In the "App Settings" section, select the "Advaned" option</li>
  <li>Enable "Developer Mode" and exit the settings menu</li>
  <li>Select your profile icon in the bottom-left corner and click "Copy User ID</li>
  <li>Provide this to the WindowsGSM admin</li>
</ol>

#### Add Admin User to WindowsGSM
<ol>
  <li>Go to the Discord tab in WindowsGSM</li>
  <li>Click "ADD ADMIN ID" in the upper-right</li>
  <li>Paste in the ID provided from above<br><b>By default, the admin will have permissions to manage all servers. If they should only have permissions for specific servers, continue to the next step. Otherwise, stop here.</b></li>
  <li>Click "EDIT SERVER ID" in the upper-right</li>
  <li>Provide a list of server IDs they should be able to manage using the provided sample format![image](https://github.com/WindowsGSM/Documentation/assets/49689423/2960d96f-72fc-4f69-bbf8-399fd2b421c2)
</li>
</ol>

## Discord Webhooks
These are used to provide notifications for server status changes. Webhooks are setup per server in WindowsGSM. This allows for setting up a webhook per channel in Discord per server
