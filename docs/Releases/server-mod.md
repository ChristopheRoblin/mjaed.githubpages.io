---
layout: default
has_children: false
title: Server framework
nav_order: 
published: false

---
# Server framework

1. Installation instructions
2. For mod creators
3. Changelog

## 1. Installation instructions

[Download the mod](/assets/images/art.zip){: .btn .fs-5 .mb-4 .mb-md-0 .mr-2 }

Copy the art.zip without unpackaging it to your servers root directory (same directory as ddct_dcm_yoserver.exe, main.cs and config_local.cs)

You are now set to download install and use compatible mods to the server framework

## 2. For mod creators

Please visit our documentation [here](#docs)

## 3. Changelog


| Date | Version | Comment |
| --- | --- | --- |
| 01.12.2021 | 2.6.1| Added multiple hooks to support registration of player death and rudementery anticheat. |
| 15.04.2021 | 2.4.0 | Added display of new version tag on modsAdded inclution of Utility a public repository for common functions to the LiFx framework |
| 30.01.2021 | 2.2.0 | Added new hooks$LiFx::hooks::onPostConnectRoutineCallbacks = JettisonArray(“onPostConnectRoutineCallbacks”);$LiFx::hooks::onPreConnectRequestCallbacks = JettisonArray(“onPreConnectRequestCallbacks”); |
| 24.01.2021 | 2.1.0 | Released, 1.x.x is now deprecated and unsupported |
| 02.01.2021 | 2.0.0 | See Server autoloader 2.0.0 |
| 27.12.2020 | v1.1.0 | Introduced a new config file in mods/AutoloadConfig.csEach mod has 4 settings-1 = Uninstall – remove all associated files*0 = Do nothing – excisting files will remain intact1 = Download but do not execute // Enables mod2 = Download and execute **All settings will be unpacked with 0 as their default setting* uninstall is not implemented** execution as per now is for future use and does not apply to third party mods, is currently only used for LiFx main mod. |
| 21.12.2020 | v1.0.3 | Changed when db.cs is executed to before InitServer to append sql to dump.sql |
| 21.12.2020 | v1.0.2 | Added initServer calls that will execute “db.cs” files in mods/<yourmod>/db.cs just before CreateServer starts for adding SQL updates after dump.sql and patch.sql has ranAdded overloadable init call for starting packages loaded after onStart() |
| 20.12.2020 | v1.0.1 | Added onPostInit call |
| 19.12.2020 | v1.0.0 | The initial release of our server-side mod, it introduces our LiFx Mod Framework structure |