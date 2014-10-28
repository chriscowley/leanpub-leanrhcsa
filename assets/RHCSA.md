# Introduction
Preparation for Red Hat Certified System Administrator (RHCSA) Exam objectives (EX200).

## What you need
This is a difficult one, the answer is it depends. Ihere is very little in this exam that cannot be learnt with nothing but a couple of Virtual Machines. The exception is the control of Virtual Machines and some of the file system work.

The simplest option is to use Oracle VirtualBox. It is free and works on Windows, Linux and OSX. Having said that, personally I use KVM while on Linux.

If you have access to VMware, then brilliant, but not all the free options are suitable.ESXi would require extra hardware so many not work for you, and VMware Player only allows you to run a single VM, it will be fine for some stuff, but not others.

You do not really need a subscription to RHEL. Red Hat are one of the best Open Source companies out there. Not only do they publish the source code, the publish it all as packages that make building your own RHEL relatively trivial. The two main projects that do this are [CentOS](www.centos.org) and [Scientific Linux](https://www.scientificlinux.org/). Of the two I tend towards CentOS, not for any particular reason, I just do. Make your choice, but there is no real need to stick with it.

# The Basics

## Access a shell prompt and issue commands with correct syntax.
The shell prompt is the core of the RHEL experience (and Linux in general). Simply this is because the majority of systems are headless servers. These will not generally have a desktop environment installed.

In the case, access a prompt is very simple. You walk up to the console and log in.
![](https://dl.dropboxusercontent.com/u/10111478/console-screenshot.png)

## Use input-output redirection (>, >>, |, 2>, etc.)
Input/output redirection is the way of controlling where a command's output goes and where it gets input from. 

* STDIN - standard input
* STDOUT - standard output
* STDERR - standard error

Both STDOUT and STDERR are outputs, the difference being the convention of what goes to each. It is pretty self-explanatory really. If it is an error message it goes to STDERR, everything else goes to STDOUT.

The best way to explain how to use this is with examples.

```
cat /etc/passwd > testfile
```

## Use grep and regular expressions to analyze text.
## Access remote systems using ssh and VNC.
## Log in and switch users in multiuser runlevels.
## Archive, compress, unpack, and uncompress files using tar, star, gzip, and bzip2.
## Create and edit text files.
## Create, delete, copy, and move files and directories.
## Create hard and soft links.
## List, set, and change standard ugo/rwx permissions.
## Locate, read, and use system documentation including man, info, and files in /usr/share/doc.


# Operating a System

##    Boot, reboot, and shut down a system normally.
##    Boot systems into different runlevels manually.
##    Use single-user mode to gain access to a system.
##    Identify CPU/memory intensive processes, adjust process priority with renice, and kill processes.
##    Locate and interpret system log files.
##    Access a virtual machine's console.
##    Start and stop virtual machines.
##    Start, stop, and check the status of network services.

# Local storage

##    List, create, delete, and set partition type for primary, extended, and logical partitions.
##    Create and remove physical volumes, assign physical volumes to volume groups, and create and delete logical volumes.
##    Create and configure LUKS-encrypted partitions and logical volumes to prompt for password and mount a decrypted file system at boot.
##    Configure systems to mount file systems at boot by Universally Unique ID (UUID) or label.
##    Add new partitions and logical volumes, and swap to a system non-destructively.

# File Systems

##    Create, mount, unmount, and use ext2, ext3, and ext4 file systems.
##    Mount, unmount, and use LUKS-encrypted file systems.
##    Mount and unmount CIFS and NFS network file systems.
##    Configure systems to mount ext4, LUKS-encrypted, and network file systems automatically.
##    Extend existing unencrypted ext4-formatted logical volumes.
##   Create and configure set-GID directories for collaboration.
##    Create and manage Access Control Lists (ACLs).
##    Diagnose and correct file permission problems.

# Configure Systems

##    Configure networking and hostname resolution statically or dynamically.
##    Schedule tasks using cron.
##    Configure systems to boot into a specific runlevel automatically.
##    Install Red Hat Enterprise Linux automatically using Kickstart.
##    Configure a physical machine to host virtual guests.
##    Install Red Hat Enterprise Linux systems as virtual guests.
##    Configure systems to launch virtual machines at boot.
##    Configure network services to start automatically at boot.
##    Configure a system to run a default configuration HTTP server.
##    Configure a system to run a default configuration FTP server.
##    Install and update software packages from Red Hat Network, a remote repository, or from the local file system.
##    Update the kernel package appropriately to ensure a bootable system.
##    Modify the system bootloader.

# Users and Groups

##    Create, delete, and modify local user accounts.
##    Change passwords and adjust password aging for local user accounts.
##    Create, delete, and modify local groups and group memberships.
##    Configure a system to use an existing LDAP directory service for user and group information.

# Security

##    Configure firewall settings using system-config-firewall or iptables.
##    Set enforcing and permissive modes for SELinux.
##    List and identify SELinux file and process context.
##    Restore default file contexts.
##    Use boolean settings to modify system SELinux settings.
##    Diagnose and address routine SELinux policy violations.

