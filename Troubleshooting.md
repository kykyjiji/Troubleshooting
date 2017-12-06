### [Excellent Firefox Privacy Add-ons](https://privacytoolsio.github.io/privacytools.io/#addons) ###
***

**Firefox Release  45.0 March 8, 2016:**

Introduce a new preference (network.dns.blockDotOnion) to allow blocking .onion at the DNS level.

The new "feature" is _enabled_ by default to block .onion addresses.

**Browser Error:**

"Server not found" "Firefox can’t find the server at abcxyz.onion" and "problems loading page"

**The Browser Fix:**

`about:config`

Search: blockDotOnion

**Change from: true**

`network.dns.blockDotOnion user set   boolean  true`

**[Change to: false](https://drive.google.com/open?id=0B79r4wTVj-CZSkZieEVCWUtKRVE)**

`network.dns.blockDotOnion user set  boolean false`


[**Disable IPv6 Privacy Extension in Linux**](https://www.binarylane.com.au/support/solutions/articles/1000100519-disable-ipv6-privacy-extension-in-linux)


### Distro Specific Fix:
* [Arch Linux](https://github.com/ruped24/toriptables2/pull/5/files)
```bash
sed -i 's/debian-tor/tor/' toriptables2.py
```
* [Parrot Security OS 3.1.1 Anonsurf](https://www.inforge.net/xi/threads/parrot-security-os-3-1-1-anonsurf-fix-tor-by-vap0r.457379/) *Note: Translation needed*
* [Tor-user on Other Distros](https://github.com/GouveaHeitor/nipe/blob/master/lib/Nipe/Device.pm) *Note: Perl code reading needed*
* [Notification error](https://wiki.archlinux.org/index.php/Desktop_notifications)
```bash
sudo apt-get install mate-notification-daemon 
```
***
### Frequently Asked Questions:
Q. Is there an easier way to install toriptables2 without all the command-line hacking?

A. Not at this time.  Hopefully in the future the Kali Gods will add **toriptables2** to [Kali Linux repo](https://bugs.kali.org/view.php?id=3983).

Q. I was looking for something that's easy to install that will give anonymity and work on Windows.

A. Installing the [Tor Browser](https://www.torproject.org/projects/torbrowser.html.en) probably would be the path of least resistance.

Q. I see it's written in Python.  Will it work on Windows?

A. Not at this time.  Iptables is not native to Windows.
   At the rate Microsoft is making [Windows more Linux like](https://msdn.microsoft.com/en-us/commandline/wsl/faq), maybe in the near future...

Q. Why do I get an IPv6 Address and [whatismyipaddress](https://whatismyipaddress.com/) shows [my real location](https://www.internetsociety.org/resources/deploy360/2014/privacy-extensions-for-ipv6-slaac/)?

A. [**Disable IPv6**](http://ask.xmodulo.com/disable-ipv6-linux.html) at the OS level.
 
1.  sysctl -w net.ipv6.conf.default.disable_ipv6=1

1.  sysctl -w net.ipv6.conf.all.disable_ipv6=1

Q. Is Tor Really Anonymous?

A. Well, I'll leave you with [this](http://lmgtfy.com/?q=Is+Tor+Really+Anonymous).