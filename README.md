#	On Ac Power State Change

This is a simple script that will run any command you choose, whenever your power state changes (ie: When your laptop power is unplugged or plugged back in). Should run correctly under any user. 

##	Requirements

* Bash, obviously
* "logger" should be installed, so this tool can add system logs
* "acpi" should be installed, so this tool can detect power state changes
	* (only tested with version 1.7)

##	Usage

Usage is pretty simple. Just pass your custom command as arguments, like so:

```
$ on-ac-power-state-change echo "Yay this works!"
```

At that point, you should see the message "Yay this works!" appear in the console whenever your power state changes. This is commonly when a laptop's power cable has been unplugged, or plugged back in.


##	Cautions

Because this tool will execute **any** command you provide, it might not be very safe to run as root or an important account unless you know what you're doing.

##	License
Released under the [Mit License](https://opensource.org/licenses/MIT)



