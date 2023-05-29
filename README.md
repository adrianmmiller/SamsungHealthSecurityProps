# Samsung Health Security Props

You may wish to try this method instead https://github.com/BlackMesa123/KnoxPatch, as its maintained, whereas this module, is not


Removes "**sakv2**" from **ro.security.keystore.keytype** to help make Samsung Health run on rooted Samsung devices. This doesnt mean its a universal "fix" and works on every device every time, so ymmv....

Notice: I am switching back to Pixel after becoming way too frustrated at the bullshit Samsung makes you go through to use the devices you pay them a tonne of money in the way you chose to do. Hours and hours of my life have been wasted because of Samsung. The owner should be able to use any device they have bought any way they like in my opinion. Almost every update Samsung tries to stop root users using simple things like health apps (why?) or to connect their watch on a rooted device, and i got tired of this bastardry.  There was a time early on in Android where Samsung had tolerance for developers, but now they just want to control peoples devices like fucking Apple, the lowest of the low of companies, and ive had enough of the race to the bottom. No more money will be going from me to Samsung, they can get fucked. As such i will not actively be maintaining this module or testing ways to beat whatever bullshit Samsung tries to block you from using your own devices....i will only respond to issues with the current module

Disclaimer:  The changes made by this module may have ramifications/consequences beyond what you may be using it for (Samsung 
Health). I have tested it for several days and havent found any personally, but this doesnt mean they dont exist. You use this at your 
own risk

This module:

- looks for **/vendor/build.prop**
- if found, it copies the **ro.security.keystore.keytype** line (in case not everyone has the same keytypes in the line - i hate using 
static files, i write modules to use whats on each device) to a new **system.prop** file in the modules folder 
- removes **sakv2** from the line in **system.prop** (it will remove sakv2 from the line (hopefully) wherever it exists, beginning, end or middle)

I had planned to test this new "fix" for a while before releasing the module to stop people from manually editing the existing file, as using 
magisk is preferable as its easily reversible, but once i saw posts on XDA about it, i figured id release this now

As mentioned above, there may be side effects to this "fix", ymmv

Note: You still need to make sure you have Samsung Health added to Magisk's Deny List, ideally with Shamiko installed (if using Shamiko dont forget to disable Enforce Deny List)


**Please note:** the included LICENSE only covers the module components provided by the excellent work of Zack5tpg's Magisk Module Extended, which is available for here for module creators

https://github.com/Zackptg5/MMT-Extended/

All other work is credited (where possible) above and **no one may fork or re-present this module as their own for the purposes of trying to monetize this module or its content without all parties permission. The module comes specifically without an overall license for this intent.**


### Project Stats ###

![GitHub release (latest by date)](https://img.shields.io/github/v/release/adrianmmiller/SamsungHealthSecurityProps?label=Release&style=plastic) ![GitHub Release Date](https://img.shields.io/github/release-date/adrianmmiller/SamsungHealthSecurityProps?label=Release%20Date&style=plastic) ![GitHub Releases](https://img.shields.io/github/downloads/adrianmmiller/SamsungHealthSecurityProps/latest/total?label=Downloads%20%28Latest%20Release%29&style=plastic) ![GitHub All Releases](https://img.shields.io/github/downloads/adrianmmiller/SamsungHealthSecurityProps/total?label=Total%20Downloads%20%28All%20Releases%29&style=plastic)
