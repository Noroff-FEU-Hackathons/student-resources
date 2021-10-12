# Linux-directory-structure 

### Introduction :

* `/` - This is the top level root directory, that contains all other directories on the system.
* `bin` - This directory contains all the essential binary executable programs, required for booting, shells like cp, ls, grep, kill, [vi text editor](https://en.wikipedia.org/wiki/Vi) etc.
* `boot` - All of the static files used in booting the system are located here e.g [grub](https://en.wikipedia.org/wiki/GNU_GRUB), [vmlinux](https://en.wikipedia.org/wiki/Vmlinux)
* `cdrom` - It is not part of the Filesystem hierarchy standard but can be found usually in Ubuntu. It is used as a temporary location for CD-ROMs.
* `dev` - Files related to the hardware as cdrom, cpu, drive can be found here. Also some pseudo-devices as `dev/null`.
* `etc` - Host-specific system configuration files.
* `home` - This is the home directory for each user on the system e.g /home/user1, /home/user2 that contains configurations per user.
* `lib` - All of the shared library images and kernel modules needed by /bin and /sbin.
* `lost+found ` - All of the unlinked, corrupted files used to recover by [fsck](https://en.wikipedia.org/wiki/Fsck) are placed here.
* `media` - All of the removable media as CD, USB when plugged into the system are mounted inside the media directory.
* `mnt` - This is used for a temporary mounting file system.
* `opt` - This directory contains optional packages and third party applications.
* `proc` - It contains the information related to the running processes.
* `root` - The home directory for the root user.
* `sbin` - Similar directory as /bin that contains essential binaries for system administration.
* `srv` - This directory contains most of the service related or files specific to servers.
* `sys` - The virtual file system.
* `usr` - All of the files used by the users, not by the system are saved in this directory.
* `var` - It contains most of the variable data files as logs, mails, temp files.

### Exploring directories and their usability :

>We know that Linux is a very complex system that requires an efficient way to start, stop, maintain and reboot a system, unlike Windows operating system. In the Linux system some well-defined configuration files, binaries, man pages information files available for every process. 

#### Linux Kernel File:

   -  /boot/vmlinux–The Linux kernel file

#### Device Files:

   - /dev/nvmeXX – Device file for the first IDE SSD (XX signifies the number).
   - /dev/hdc – A pseudo-device that output garbage output is redirected to /dev/null.

#### System Configuration Files:

  -  /etc/bashrc – It is used by bash shell that contains system defaults and aliases.
  -  /etc/crontab – A shell script to run specified commands on a predefined time interval.
  -  /etc/exports – It contains information on the file system available on the network.
  -  /etc/fstab – Information of the Disk Drive and their mount point.
  -  /etc/group – It is a text file to define Information of Security Group.
  -  /etc/grub.conf – It is the grub bootloader configuration file.
  -  /etc/init.d – Service startup Script.
  -  /etc/lilo.conf – It contains lilo bootloader configuration file.
  -  /etc/hosts – Information of IP and corresponding hostnames.
  -  /etc/hosts.allow – It contains a list of hosts allowed accessing services on the local machine.
  -  /etc/host.deny – List of hosts denied to access services on the local machine.
  -  /etc/inittab – INIT process and their interaction at the various run level.
  -  /etc/issue – Allows editing the pre-login message.
  -  /etc/modules.conf – It contains the configuration files for the system modules.
  -  /etc/motd – It contains the message of the day.
  -  /etc/mtab – Currently mounted blocks information.
  -  /etc/passwd – It contains username, password of the system, users in a shadow file.
  -  /etc/printcap – It contains printer Information.
  -  /etc/profile – Bash shell defaults.
  -  /etc/profile.d –  It contains other scripts like application scripts, executed after login.
  -  /etc/rc.d – It avoids script duplication.
  -  /etc/rc.d/init.d – Run Level Initialisation Script.
  -  /etc/resolv.conf – DNS being used by System.
  -  /etc/securetty – It contains the name of terminals where root login is possible.
  -  /etc/skel – Script that initiates new user home directory.
  -  /etc/termcap – An ASCII file that defines the behavior of different types of the terminal.
  -  /etc/X11 –  Directory tree contains all the conf files for the X-window System.

#### User Related Files:

   - /usr/bin – It contains most of the executable files.
   - /usr/bin/X11 – Symbolic link of /usr/bin.
   - /usr/include – It contains standard include files used by C program.
   - /usr/share – It contains architecture independent shareable text files.
   - /usr/lib – It contains object files and libraries.
   - /usr/sbin – It contains commands for Super User, for System Administration.

#### Virtual and Pseudo Process Related Files:

 -    /proc/cpuinfo – CPU Information
 -    /proc/filesystems – It keeps the useful info about the processes that are running currently.
 -    /proc/interrupts – it keeps the information about the number of interrupts per IRQ.
 -    /proc/ioports – Contains all the Input and Output addresses used by devices on the server.
 -    /proc/meminfo –  It reports the memory usage information.
 -    /proc/modules – Currently using kernel module.
 -    /proc/mount – Mounted File-system Information.
 -    /proc/stat –  It displays the detailed statistics of the current system.
 -    /proc/swaps –  It contains swap file information.

#### Version Information File:

    /version – It displays the Linux version information.

#### Log Files:

    /var/log/lastlog – It stores user last login info.
    /var/log/messages – It has all the global system messages.
    /var/log/wtmp – It keeps a history of login and logout information.

>To check the Linux directories open the terminal and execute sudo -s followed by system password to give root privilege. Then after changing the current home directory to the root directory and check the list of all available directories in the base directory as shown below. 


[For further Information](https://linuxhandbook.com/linux-directory-structure/)

[Go Back](../README.md)
