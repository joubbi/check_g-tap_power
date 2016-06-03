# check_g-tap_power

This is a script that checks the AC status of a Gigamon G-TAP-ATX.
The script logs in and connects with telnet to the tap,
then issues a "show system" and looks for the power status.
(The device doesn't support a more secure protocol)

Tested with G-TAP-ATX   Firmware Version: 2.2.27

Make sure that you have expect installed on your system.
Supply the hostname or IP address of the tap as an argument.

The script can be added to Op5 or some other Nagios like system.
Define the command like this:
```sh
check_g-tap_power.exp $HOSTADDRESS$ $ARG1$
```

Licensed under the Apache license version 2.
Written by farid.joubbi@consign.se
