# PlutosphereToolBox
Hey All, Lucas Here! I made a think that another user was working on. 
Is it stealing or enhancing? I dont know, but I wanted to make it something I can use.
And on that note, you can edit it too! (i havent made the format, but its easy to understand with some guidance)
I think after v1.1 I will leave it to the community, unless I have a big idea.
btw this is for plutosphere.com , a VR cloud gaming machine (that if you want to support me you can give me tokens at musicmanrr).
Other than that, thats all i have to say. Thank you to Deleted User#3823 for the Toolbox begining code and idea.
~
@echo off
	
cls

echo This was a ToolBox made by user Deleted User#3823 and edited by Music Man#3968. I give full credit for most of the code and the idea of this.

pause
:begining
cls
echo Welcome to plutosphere tools! what would you like to install
echo (1) - Download Parsec
echo (2) - Download Minecraft
echo (3) - Download Roblox
echo (4) - Download Virtual Desktop
echo (5) - Download Spotify
echo (6) - Download Java
echo (7) - Download Discord
echo (8) - Download Mega
echo (9) - Close
CHOICE /C 123456789 /M "Enter your choice:"
If ERRORLEVEL 9 GOTO close
IF ERRORLEVEL 8 GOTO Mega
IF ERRORLEVEL 7 GOTO Discord
IF ERRORLEVEL 6 GOTO Java
IF ERRORLEVEL 5 GOTO Spot
IF ERRORLEVEL 4 GOTO VDSK
IF ERRORLEVEL 3 GOTO rblx
IF ERRORLEVEL 2 GOTO mine
IF ERRORLEVEL 1 GOTO psec 

:Mega
cls
echo Installing
curl https://mega.nz/MEGAsyncSetup64.exe -o mega.exe
cls
start mega.exe
GOTO end

:Discord
cls
echo Installing
curl https://discord.com/api/downloads/distributions/app/installers/latest?channel=stable&platform=win&arch=x86 -o discord.exe
cls
start discord.exe
GOTO end

:Java
cls
echo Installing
curl https://javadl.oracle.com/webapps/download/AutoDL?BundleId=246471_2dee051a5d0647d5be72a7c0abff270e -o Java.exe
cls
start Java.exe
GOTO end

:Spot
cls
echo Installing
curl https://download.spotify.com/SpotifyFullSetup.exe -o spot.exe
cls
start spot.exe
GOTO end

:vdsk
cls
echo Installing
curl https://download.vrdesktop.net/files/VirtualDesktop.Streamer.Setup.exe -o vdsk.exe
cls
start vdsk.exe
del Parsec.zip

:rblx
cls
echo Installing
curl https://setup.rbxcdn.com/version-c1236188328f4133-Roblox.exe -o rblx.exe
cls
start rblx.exe
GOTO end

:mine
cls
echo Installing
curl https://launcher.mojang.com/download/MinecraftInstaller.msi -o mine.msi
cls
start mine.msi
GOTO end

:psec
cls
echo Installing
curl https://builds.parsecgaming.com/package/parsec-flat-windows32.zip -o Parsec.zip
cls
tar -xf Parsec.zip
timeout 3 /NOBREAK > nul
del Parsec.zip
cd parsec
start parsecd.exe
GOTO end

:end
cls
echo Task Finshed! Either:
echo (1) - Download another app
echo (2) - Close App
CHOICE /C 12 /M "Enter your choice:"
IF ERRORLEVEL 2 GOTO close
IF ERRORLEVEL 1 GOTO begining 

:close
cls
echo Press any key to close app.
pause
 ~
