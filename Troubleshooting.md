### [Excellent Firefox Privacy Add-ons](https://privacytoolsio.github.io/privacytools.io/#addons) ###
***

**Firefox Release  45.0 March 8, 2016:**

Introduce a new preference (network.dns.blockDotOnion) to allow blocking .onion at the DNS level.

The new "feature" is _enabled_ by default to block .onion addresses.

**Browser Error:**

"Server not found" "Firefox can’t find the server at abcxyz.onion" and "problems loading page"

**The Fix:**

`about:config`

Search: blockDotOnion

**Change from: true**

`network.dns.blockDotOnion user set   boolean  true`

**[Change to: false](https://drive.google.com/open?id=0B79r4wTVj-CZSkZieEVCWUtKRVE)**

`network.dns.blockDotOnion user set  boolean false`


### Distro Specific Fix:
* [Parrot Security OS 3.1.1 Anonsurf](https://www.inforge.net/xi/threads/parrot-security-os-3-1-1-anonsurf-fix-tor-by-vap0r.457379/) *Note: Translation needed*
* [Arch Linux](https://github.com/ruped24/toriptables2/pull/5/files)
* [Notification error](https://wiki.archlinux.org/index.php/Desktop_notifications)
```
#!bash
sudo apt-get install mate-notification-daemon 
