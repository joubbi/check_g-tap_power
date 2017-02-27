# check_g-tap_power

This is a script that checks the AC status of a __Gigamon G-TAP-ATX__.
The script logs in and connects with telnet to the tap,
then issues a "show system" and looks for the power status.
(The device doesn't support a more secure protocol)

Tested with G-TAP-ATX Firmware Version: 2.2.27

Make sure that you have expect installed on your system.
Supply the hostname or IP address of the tap as an argument.

The script can be added to Op5 or some other Nagios like system.
Define the command like this:
```sh
check_g-tap_power.exp $HOSTADDRESS$ $ARG1$
```

## Version history:
* 1.1 2016-06-02 Minor cleanup of dialogues and help.
* 1.0 2015-10-23 Initial version.
___

Licensed under the [__Apache License Version 2.0__](https://www.apache.org/licenses/LICENSE-2.0)

Written by __farid@joubbi.se__

http://www.joubbi.se/monitoring.html

