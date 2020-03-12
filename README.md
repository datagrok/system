# system

a repo for miscellaneous system-level configuration files, cronjobs and executable scripts. some examples:

- `usr/local/sbin/adduser.local`: an example of how to customize `adduser` to automate the creation of password-less users who can log in using their public ssh keys.
- `etc/etc-services-nfs.txt`: ports commonly used for the different nfs daemons
- `etc/cron.weekly/lvmscrub`: i have an lvm raid. this invokes a weekly "scrub" which tests the array for data corruption, hopefully before too much has become corrupted to recover from.
- `etc/cron.daily/library-backup`: how i used to create a local backup of my media server (now i use restic with backblaze b2)
- etc/X11/Xsession.d/999custom_userxprofile: make X11 look for and source ~/.xprofile on login
- `etc/X11/xorg.conf.d/99-logitech-m570-wireless-trackball.conf`: make my Logitech m570 work the way I like it; where the "right button" triggers scroll-wheel mode and the left, middle, and right buttons are all reachable with the pointer finger
- `etc/X11/xorg.conf.d/99-logitech-trackball.conf`: make my Logitech TrackMan Marble work the way I like it; where the "thumb button" triggers scroll-wheel mode, and left- and middle-click are all reachable with the middle finger.
