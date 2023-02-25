# T7 Server Config
Config for T7 Dedicated Servers for use with the BOIII Client.

# How to use
1. Download the BO3 Unranked Dedicated Server via Steam (it's located in the "Tools" section in your library)
2. Open the Unranked Server folder in windows explorer (if you own BO3 on Steam and have it installed it will be in your BO3 Game Folder)
3. Add boiii.exe to the Unranked Server Folder
4. Download this repository and move the startup batch files as well as the zone folder to the Unranked Server Folder
5. Edit the config in /zone to your liking
6.(Optional) (Skip step 9 when using this) Download https://mega.nz/folder/zY80VTyC#bAdFvhRtaTrlxUslCkkngg as zip and extract all contents in /zone

As of right now you need to take additional Steps to host Zombies Servers, this may change in future Updates of BOIII.

7. Create the following Folder Structure inside the Unranked Server Folder:
```
boiii/lobby_scripts/zombie
```
8. [Get this LUA Script](https://github.com/JezuzLizard/T7-18-Player-Dedicated-Zombies-Server-Mod/blob/main/server/ui_scripts/zombies_server_mod/__init__.lua) and move it into the ```zombie``` Folder. The entire Path should now look like this:
```
Unranked Server/boiii/lobby_scripts/zombie/__init__.lua
```
9. For Zombie Dedis to work they need to have the Zombies Maps and common FastFiles, these do not come with the Unranked Server Files. This means you need to copy those over from your BO3 Game Folder.

Copy:
```
zone/zm_common.fd
zone/zm_common.ff
zone/zm_levelcommon.ff
```
from your BO3 Game folder into the Unranked Server's ```zone``` Folder. Do the same with the FastFiles of the Maps you want to host on the Server, you do not need to copy the .xpak files, those hold Textures and Sounds which the Server doesn't need.

10. You are now ready to start the Server using BOIII_ZM_Server.bat.
