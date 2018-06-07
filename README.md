# check_debian_restarts
Shows if your system or service needs a restart because it is using old files/libs - its just a wrapper for /usr/sbin/checkrestart
Installation:
```
# you need the debian-goodies package
aptitude install debian-goodies
```

You need a sudo config for this script:

```
cat /etc/sudoers.d/nagios
nagios ALL = NOPASSWD: /usr/lib/nagios/plugins/check_debian_restarts
```
