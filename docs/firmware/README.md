## Firmwares

### Normal

#### Mini-Motion-3232 (2024-07-27)

3232 is the normal / non-customized version used for WSW custom firmware (9008).



#### Mini-Motion-3231 (2024-07-06)

3231 is the normal / non-customized version used for WSW custom firmware (9007).

- Collection of bug fixes.
- 10Hz is back but enabling it will forever reduce the battery life of the device by 15%, even if you switch back to 5Hz after.
- Upgraded the terrain/street map on the device's embedded website.
- Slightly reduced WiFi reach to avoid power consumption spikes.



#### Mini-Motion-3212 (2023-10-06)

3212 is the normal / non-customized version used for WSW custom firmware (9004 + 9005).



#### Mini-Motion-3190 (???)

Simplifies and clarifies timezones, speed units and distance units.

[LCD] Brings back live configuration of brightness, timezone, speed unit and distance unit.



#### Mini-Motion-3183 (???)

Fixes an end of run detection issue.



#### Mini-Motion-3181 (2022-11-09)

Added HDOP to GPX.



#### Mini-Motion-3178 (2022-11-01)

Fix 1 Hz logging issue on M8 devices (3176 or 3177).

Also includes a sync attempt.



#### Mini-Motion-3177 (2022-10-31)

Handle slow alphas using the 10s average for the speed filter, instead of current speed (3176).



#### Mini-Motion-3175 (2022-10-09)

Fixes issue that could cause mini to lock up and unable to restart, requiring ~24 hours of wait.



#### Mini-Motion-3174 (2022-10-08)

Includes features of 9002 (WSW)

Untrustworthy WiFi networks can now be forbidden from editing or deleting data (3171).



#### Mini-Motion-3170 (2022-10-05)

In worst case scenarios, devices will now restart and resume logging on their own.



#### Mini-Motion-3168 (2022-10-03)

M8 and M10 are now PMS "Full", instead of "Balanced" which is the default. There is a warning about "Balanced" in the u-blox docs.

Full/Balanced on the M8 didn't make any difference in testing, so Motion originally went with the default of "Balanced".

10 is now LNA Normal. 8 LNA can't be configured. #3144

There's several of your requests in it but not the logging watchdog. Noticed the 3 flashes every 10 seconds during charging.



#### Mini-Motion-3159 (2022-10-02)

Received whilst in Welwyn so not tested. Went straight to 3168.



#### Mini-Motion-3151 (2022-09-29)

Response to devices switching off. No improvement.



#### Mini-Motion-3144-bypass (2022-09-25)

Battery scale improvement. #3130

LNA Normal. #3142

Note: Static spikes eliminated but sAcc higher



#### Mini-Motion-3129 (~2022-08-11)

Allows many more different characters in the board, sail, fin, etc fields. #3124

Fixes two minor issues in Alpha 500m. #3124



#### Mini-Motion-3120

Provided by Julien for static testing of 633 and 634 after spikes were discovered on 633 and 634 using 3130.



#### Mini-Motion-3118 (2022-07-27)

Alpha 500m corrections according to V2 example #3115 

Alpha 500m is now full-Hz #3116

Min speed is 1 m/s. #3117



#### Mini-Motion-3111 (~2022-07-09)

10 second flasher. #3110



#### Mini-Motion-3109 (2022-07-09)

It comes with your alpha, WiFi connection to your own networks*, a constant LED blinker, custom LED blinking of various speeds**, a revamped web server, a panic restart on 12+ button presses and an easier way to access the webserver

*: connect to the WiFi as usual by pressing the button twice, go to the webserver settings, make sure to refresh the page, enter your WiFi login/password, press the button twice to exit WiFi mode.

​     From now on, you can press the button three times to enter the new WiFi mode. It will blink red/green while searching for your networks, then blink red/green while connecting to it, then stay green forever if connected. Or show red for a few seconds and stop if it couldn't connect. The device will still be active. Your login/password might be wrong or your own WiFi router might be too far.

 **: for example, it will blink your "over 10s #1 run" on four button presses. To be configured in the settings.

Warning: it will forget your current settings.



#### Mini-Motion-3085 (2022-05-28)

#3084 had a tiny bug where a fully charged battery would be reported as half charged.



#### Mini-Motion-3084 (2022-05-26)

GPX fixes - back to 1.0



#### Mini-Motion-3068

Version shipped with motion-470.



### Custom

#### Mini-Motion-9010 (2024-10-04)

Based on 3232 release.

Includes some additional Motion identifiers (2023 devices).



#### Mini-Motion-9009 (2024-10-04)

Based on 3232 release.

Includes some additional Motion identifiers.



#### Mini-Motion-9008 (2024-07-27)

Based on 3232 release.



#### Mini-Motion-9007 (2024-07-06)

Based on 3231 release.

- It has a 2s > 3kn filter.
- Core bug fixes.
- Button press detection changes.
- Power assigned to WiFi is a bit lower.



#### Mini-Motion-9005 (2023-10-06)

Based on 3212 release.

Special 2 knot minimum for youths.



#### Mini-Motion-9004 (2023-09-30)

Based on 3212 release

Includes WSW device numbers.



#### Mini-Motion-9003 (2022-10-14)

Based on 3175 release.



#### Mini-Motion-9002 (2022-10-07)

Correct WiFi password and edition/deletion forbidden.



#### Mini-Motion-9001 (2022-10-06)

New list of devices:

> 601 611 615 617 618 619 621 625 630 631 632 633 634 635 639 656



#### Mini-Motion-9000 (2022-10-06)

First WSW release, presumably based on 3170.

Any Mini/LCD on firmware 9000 Weymouth:
- 5Hz
- 5kn min
- UTC+1
- WSW WiFi

Any Mini on firmware 9000 Weymouth:
- Blinker on

Minis that are WSW on firmware 9000 Weymouth (so far these are only 470, 619, 621, 633, 634):
- name WSW
- kn speed
- km distance
- 500m last, 500m best, 250m last, 250m best speed blinkers with 0 subtraction so 26kn = 2 red + 6 green blinks

