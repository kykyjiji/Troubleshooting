## [Installation options after downloading or cloning](https://www.youtube.com/watch?v=3mEpnzY5ZZo&feature=youtu.be)

### Executing toriptables2.py as a standalone executable:

1. `sudo cp -var toriptables2.py /usr/local/bin/`

1. `cd /usr/local/bin`

1. `sudo chown root.root toriptables2.py`

1. `sudo chmod +x toriptables2.py`

1. `cd ~ `

1. `sudo toriptables2.py -h`

```
usage: toriptables2.py [-h] [-l] [-f]

Tor Iptables script for loading and unloading iptables rules

optional arguments:
  -h, --help   show this help message and exit
  -l, --load   This option will load tor iptables rules
  -f, --flush  This option flushes the iptables rules to default
```

### Executing toriptables2 module as a script:

1. `sudo cp -var toriptables2.py /usr/local/lib/python2.7/dist-packages/`

1. `cd /usr/local/lib/python2.7/dist-packages`

1. `sudo chown root.staff toriptables2.py`

1. `sudo chmod 644 toriptables2.py`

1. `cd ~`

1. `sudo python -m toriptables2 -h`

```
usage: toriptables2.py [-h] [-l] [-f]

Tor Iptables script for loading and unloading iptables rules

optional arguments:
  -h, --help   show this help message and exit
  -l, --load   This option will load tor iptables rules
  -f, --flush  This option flushes the iptables rules to default
```
```
┌─[mint@mint]─[~]
└──╼1 (00:03:16) >> sudo python -m toriptables2 -l
 [+] Anonymizer status [ON]
 [*] Getting public IP, please wait...
 [+] Your IP is 185.38.14.171
┌─[mint@mint]─[~]
└──╼2 (00:03:39) >>
```