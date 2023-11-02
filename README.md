# WindowsGSM.ArkSurvivalAscended
🧩WindowsGSM plugin that provides Ark Survival Ascended Dedicated server support!

## Requirements

This plugin was developed and tested with WindowsGSM version 1.23.1. No guarantee that it will work on anything below that.

## Installation

1. Download the repo as zip
2. Copy the **ArkSurvivalAscended.cs** folder into the WindowsGSM/plugins folder
3. Reload the plugins.


## Ark server parameters

Example paramters below:

**WARNING: Note this is just an example, do not use this on your production server**

```
?RCONEnabled=True?RCONPort=27021 -lowmem -nosteamclient -game -ActiveEvent=None -nosound -sm4 -server -log -servergamelog -ServerRCONOutputTribeLogs -nitradotest -culture=en -EnableSteelShield -pconlymods -ServerPlatform=PC -servergamelogincludetribelogs -nobattlEye -UseDynamicConfig -NotifyAdminCommandsInChat -Mods=914844 -automanagedmods -forcerespawndinos
```

The easiest way to check if the parameters are working, is to change the default port, start the server and then do a
```
netstat -an
```

Look for your changed port listening. If it is, everything works. If it's 7777, then you're running without any/most of the parameters.

## Installing and running mods

EDIT: Please add -automanagedmods as well!!!!

You will need to add the following parameter:

```
-Mods=XXXX,XXXX,XXXX
```

The XXXX is the mod ID's.

To check all the mods available, and find their ID's, go to:

[CurseForge ASA Mods](https://www.curseforge.com/ark-survival-ascended)

Clicking on a mod, will reveal the mods details and you can find the "Project ID" on the right side. The number is the ID you need to put in the -Mods parameter.

## License
Software is provided as is. If your server explodes, i will deny everything. If it makes you a coffee, send some my way.
