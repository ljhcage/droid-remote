### droid-remote

I am wrecking my Android phones way to often by crashing them on the ground, leaving me with a dead touchscreen.
However even if wrecked an android phone is still a usable all-purpose computer. It has wireless connectivity, audio output, a camera, etc. 
There are possible use cases, if one could control - or at least re-configure it (I'd like to re-use them as webcams for instance). 
Even if you do not have any use for a phone with broken display/touchscreen, you might want to retrieve some data from it (maybe you did not make backups).

Remote controls such as VNC normally require root and do not work very well on all phones. There is a much bolder solution:
grab screenhost from the phone and send remote events via Android's debug bridge (adb). This code is inspired by 
Marian Schednig's [adbcontrol](http://marian.schedenig.name/2014/07/03/remote-control-your-android-phone-through-adb/), 
but it's written python and also handles orientation changes.

It's horribly slow - but it works.


#### Requirements:
* adb (Android SDK) installed
* Developer options and Android debbuing enabled
