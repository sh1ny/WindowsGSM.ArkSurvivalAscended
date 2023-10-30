# WindowsGSM.ArkSurvivalAscended
🧩WindowsGSM plugin that provides Ark Survival Ascended Dedicated server support!

## Requirements

This plugin was developed and tested with WindowsGSM version 1.23.1. No guarantee that it will work on anything below that.

## Installation

1. Download the repo as zip
2. Copy the **ArkSurvivalAscended.cs** folder into the WindowsGSM/plugins folder
3. Reload the plugins.


## Ark server parameters

For some reason, adding the parameters normally, will result in the server ignoring all of them. What you need to do, is leave spaces before and between each paramater. Here's an example

**WARNING: Note this is just an example, do not use this on your production server**

```
?RCONEnabled=True ?RCONPort=27021  -lowmem -nosteamclient -game -ActiveEvent=None -nosound -sm4 -server -log -servergamelog -ServerRCONOutputTribeLogs -nitradotest -culture=en -EnableSteelShield -pconlymods -ServerPlatform=PC -servergamelogincludetribelogs -nobattlEye -UseDynamicConfig -NotifyAdminCommandsInChat -automanagedmods
```

The easiest way to check if the parameters are working, is to change the default port, start the server and then do a
```
netstat -an
```

Look for your changed port listening. If it is, everything works. If it's 7777, then you're running without any/most of the parameters.

## License
Software is provided as is. If your server explodes, i will deny everything. If it makes you a coffee, send some my way.