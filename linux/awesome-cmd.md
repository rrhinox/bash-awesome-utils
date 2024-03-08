# 🐧 Linux awesome command line for day by day!

## Intro & Documentation

**What is Linux?**

Linux is a family of open-source Unix-like operating systems based on the Linux kernel, an operating system kernel first released on September 17, 1991, by [Linus Torvalds](https://github.com/torvalds). 

Linux is typically packaged as a Linux distribution (distro), which includes the kernel and supporting system software and libraries, many of which are provided by the GNU Project. Many Linux distributions use the word "Linux" in their name, but the Free Software Foundation uses and recommends the name "GNU/Linux" to emphasize the use and importance of GNU software in many distributions, causing some controversy.

[Linux.org](https://www.linux.org/)

[LinuxFoundation](https://www.linuxfoundation.org/)

[Main "distro" Donwload](https://www.linux.org/pages/download/)

[Beginner Tutorial](https://www.linux.org/forums/linux-beginner-tutorials.123/)


## Main (basic) commands 

### Access over ssh
`ssh -i /etc/pki/my-key.pem my-secure-server`

### Folder
`cd /opt/my/special/folder/to/enter` `ls -lrth /tmp`

### Files
`tail -f /var/log/syslog` `cat /etc/os-release`

`mv file-folder-to-rename desired-new-file-folder-name`

`cp file-to-copy /tmp/folder-to-copy/`

### Server process, cpu, memory and ip
`top` `ps aux` `ip addr` `vmstat` `free -h`

### Disk
`df -h` `du -h` 

## Example with some context

### Execute command over ssh write output on local path 

`ssh cluster1 'crictl logs b01edbe6f89ed' &> /opt/container.log`


