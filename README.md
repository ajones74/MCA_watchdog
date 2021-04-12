Digi APIX Watchdog Example Application
===================================

Example application to access and manage watchdog using the Digi APIX library.

This application enables a watchdog device on the board. After that, the
application starts refreshing the watchdog timer until the test time is consumed,
then the device will reboot automatically after the timeout expires.

Running the application
-----------------------
Once the binary is in the target, launch the application:

```
~# ./watchdog_app

Usage: watchdog_app <watchdog_device> <timeout> <test_time>

<watchdog_device>    Watchdog device file to manage
<timeout>            Timeout to set Watchdog timer (default 10)
<test_time>          Test duration in seconds (default 60)

```

If no arguments are provided, the example will use the default values.


Compiling the application
-------------------------
This application is meant to be compiled and deployed as part of a bitbake layer 
within the Yocto build system.

