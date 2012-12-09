# Station Storage Extension (SSE) - by Tim-O

![Station Storage Extension](http://img3.imagebanana.com/img/cxjczx2c/sse.superfreighters.jpg)

The Station Storage Extension allows to use the cargo bay of docked ships to extend the stations' storage capacity. Ships that are docked to the station and have it set as their homebase can be turned into storage extensions. They are then used to store wares if the stations' cargo bay usage exceeds a certain amount. If the station runs out of the ware at a later time, the amount stored in the extension ships is used to back it up.

The Station Storage Extension is located in the Station Command Panel. You recognize it by the yellow color.

Corresponding thread on the Egosoft forums: [[Script][Mar/13/2009]Station Storage Extension](http://forum.egosoft.com/viewtopic.php?t=239414)

## Minimum Requirements:
* A station and a docked ship with the station set as its home base.

## Installation:
* Copy the contents of the `scripts` folder into `X3 TC\scripts`
* Copy the contents of the `t` folder into `X3 TC\t`

## Update:
* Copy the contents of the `scripts` folder into `X3 TC\scripts`
* Copy the contents of the `t` folder into `X3 TC\t`
* The script will only notify you if it is currently running on a station and has to be restarted (this will be done automatically). However, you can see the current script version in the upper right corner of the main control panel. So there is where you should look to determine whether an update was successful.

## Uninstallation:
* Open a Storage Extension Control Panel in the game.
* Select the bottom item "Uninstall" and answer the following safety question with "Yes".
* Wait until the script tells you that uninstallation has been completed.
* Save.
* Quit X3.
* Remove all files of the script from the folders `scripts` and `t` (see "Used Resources")
* Done.

## Description:
Fed up with the small cargo bays of your stations and complexes? It's over now! The Station Storage Extension facilitates automatic transfer of wares to and from docked ships that have been registered with the Extenstion.
The settings allow for choosing upper and lower bounds for each ware in which the Storage Extension will try to maintain the stock. Over production is loaded into the extension ships and deficits are accounted for with the already stored cargo.
Every managed ware can be provided with preferred ships. These are then used first if some of the ware has to be stored, and last if a stock refill is necessary.
To add a ship to the list of extension ships it has to be docked at the station and have it set as its home base. You can then register the ship with the station in the "Manage Ships" section of the control panel. The ship will stay registered until it is either removed, destroyed or assigned to a different home base.
If you've got a station or complex with massive over production the Storage Extension can spare you much of the work required if you have to empty the stocks manually ever other minute or set up a complicated transport chain to a storage station. However, if the cargo bays of the extension ships should become too full at one moment the Station Storage Extension will warn you if you wish. You can set up seperate critical load levels for the cargo space of all docked extension ships and for the space used in the preferred ships of a single ware. If you really want to have a ware only in its preferred ships this will help you realize when an overflow is imminent.

## Usage:
The user interface of the Station Storage Extension should be quite intuitive to use since it was designed with that purpose in mind. Most of the windows have a descriptive text at the top that explains the settings. Just look and try and you'll understand everything quite fast. If there is any problem or unceartainty don't be afraid to ask in the script's thread in the forum.

## Used Resources:

### Command Slot:
`COMMAND_TYPE_STATION_35 (1135)`

### Language Files: 
`t\8223-L044.xml (page 8223)`
`t\8223-L049.xml (page 8223)`

`t\8910-L044.xml (page 8910)` <-------String Library by ChemODur!! http://forum.egosoft.com/viewtopic.php?t=233377
`t\8910-L049.xml (page 8910)` <-------String Library by ChemODur!! http://forum.egosoft.com/viewtopic.php?t=233377

### Script Files:
`scripts\lib.chem.strings.xml` <-------String Library by ChemODur!! http://forum.egosoft.com/viewtopic.php?t=233377

`scripts\plugin.sse.consistency.check.xml`
`scripts\plugin.sse.core.xml`
`scripts\plugin.sse.find.ship.for.loading.xml`
`scripts\plugin.sse.find.ship.for.unload.xml`
`scripts\plugin.sse.get.ware.settings.xml`
`scripts\plugin.sse.pref.usage.docked.xml`
`scripts\plugin.sse.restart.core.xml`
`scripts\plugin.sse.total.usage.docked.xml`
`scripts\plugin.sse.ui.main.xml`
`scripts\plugin.sse.ui.manage.ships.xml`
`scripts\plugin.sse.ui.manage.wares.xml`
`scripts\plugin.sse.ui.notifications.xml`
`scripts\plugin.sse.ui.ware.select.ship.xml`
`scripts\plugin.sse.ui.ware.settings.xml`
`scripts\setup.plugin.sse.xml`
`scripts\uninstall.plugin.sse.xml`

## Changelog:

### Mar 13, 2009: v beta.02

- Fixed a problem causing a freeze if a ship should unload a ware it had installed
- Fixed a problem causing "Unload and Stop" not to stop, when a ship had a ware installed it was supposed to unload

### Mar 12, 2009: v beta.01

- Initial Release
