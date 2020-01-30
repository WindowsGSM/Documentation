# Add Game Servers

This is a template game server Class, you can create a new Class base on this so WindowsGSM can support the game server.

```csharp
using System;
using System.Threading.Tasks;
using System.Diagnostics;
using System.IO;

namespace WindowsGSM.GameServer
{
    /// <summary>
    /// 
    /// Note:
    /// This is a template game server Class, you can create a new Class base on this so WindowsGSM can support the game server.
    /// 
    /// After you had created a Class:
    /// 1. Edit ClassObject.cs and add an option in the switch. (GameServer/ClassObject.cs)
    /// 2. Add FullName of the game server to List.resx (GameServer/Data/List.resx)
    /// 3. Add a 16x16 size game icon to Images/Games/
    /// 4. Add the path of game icon to Icon.resx (GameServer/Data/Icon.resx)
    /// 5. Pull request the default config to Github
    /// 
    /// Then
    /// 5. Start WindowsGSM in VS2019
    /// 6. Test install, import, start, stop, restart, updates
    /// 7. Pull request in Github
    /// 
    /// </summary>
    class __Template__
    {
        private readonly Functions.ServerConfig _serverData;

        public string Error;
        public string Notice;

        public const string FullName = ""; //FullName of the game server set in (GameServer/Data/List.resx)
        public bool ToggleConsole = false; //Set the TOGGLE CONSOLE is enable or not when server is started (Functions/ServerConsole.cs)

        public string port = ""; //The Default port of the game server
        public string defaultmap = ""; //The Default map of the game server
        public string maxplayers = ""; //The Default maxplayers of the game server
        public string additional = ""; //The addition start param which will be the serverparam value in WindowsGSM.cfg

        public __Template__(Functions.ServerConfig serverData)
        {
            _serverData = serverData;
        }

        /// <summary>
        /// 
        /// Note: Create a game server default config
        /// 
        /// </summary>
        public async void CreateServerCFG()
        {
            //Download server.cfg from github (https://github.com/WindowsGSM/Game-Server-Configs), make sure the config file is on the github
        }

        /// <summary>
        /// 
        /// Note:
        /// Check the important files before starting the server.
        /// If some important files are missing, set the error message in Error and return null.
        /// If some minor files are missing, set the notice message in Notice
        /// 
        /// If the game server in srcds.exe or hlds.exe, Steam.SRCDS or Steam.HLDS Class can be used
        /// 
        /// </summary>
        /// <returns> The process of the game server </returns>
        public async Task<Process> Start()
        {
            return null;
        }

        /// <summary>
        /// 
        /// Note: Stop the server gently
        /// 
        /// If the game server in srcds.exe or hlds.exe, Steam.SRCDS or Steam.HLDS Class can be used
        /// 
        /// </summary>
        /// <param name="p"> The process of the game server </param>
        /// <returns> is server successfully stopped </returns>
        public static async Task<bool> Stop(Process p)
        {
            return false;
        }

        /// <summary>
        /// 
        /// Note: If the game server install with steamcmd, return the steamcmd.exe process, otherwise return null
        /// 
        /// If the game server in srcds.exe or hlds.exe, Steam.SRCDS or Steam.HLDS Class can be used
        /// 
        /// </summary>
        /// <returns> The installer process. Example: steamcmd.exe. </returns>
        public async Task<Process> Install()
        {
            return null;
        }

        public async Task<bool> Update()
        {
            return false;
        }

        public bool IsInstallValid()
        {
            return false;
        }

        public bool IsImportValid(string path)
        {
            return false;
        }

        public string GetLocalBuild()
        {
            return "";
        }

        public async Task<string> GetRemoteBuild()
        {
            return "";
        }
    }
}

```

