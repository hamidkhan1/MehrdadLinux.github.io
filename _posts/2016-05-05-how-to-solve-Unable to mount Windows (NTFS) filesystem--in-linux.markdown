---
layout: post
title: "How to solve Unable to mount Windows (NTFS) filesystem"
date: "2016-03-23 15:30:20 +0430"
---

<br />some time youe need to open Windows (NTFS) filesystem in linux but you get error

```
Error mounting /dev/sda5 at /media/itsfoss/01BC76G7Z2628FB0: Command-line `mount -t “ntfs” -o “uhelper=udisks2,nodev,nosuid,uid=1000,gid=1000,dmask=0077,fmask=0177” “/dev/sda5” “/media/itsfoss/01BC76G7Z2628FB0″‘ exited with non-zero exit status 14: The disk contains an unclean file system (0, 0).
Metadata kept in Windows cache, refused to mount.
Failed to mount ‘/dev/sda5’: Operation not permitted
The NTFS partition is in an unsafe state. Please resume and shutdown
Windows fully (no hibernation or fast restarting), or mount the volume
read-only with the ‘ro’ mount option.
```


<br /> that there is some problem in windwos shutdown progress
<br /> to solve this problem you have to way
1. must disabl Fast Startup
2. use ntfsfix /dev/sdXY command<br />
<br />go to your  windows OS and do this steps :

1. Open Control Panel in the small icons view and click on Power Options.
2. Click on Choose what the power buttons do.
3. Click on Change settings that are currently unavailable.
![disable fast startup](/res/disable_fast_startup_windows8.jpeg)
4. Uncheck Turn on fast startup (recommended).
![Power-Options-in-Windows-8-1.jpeg](/res/Power-Options-in-Windows-8-1.jpeg)
<br />Click on Save changes. Now, shutdown Windows 8 and boot back into Ubuntu.
