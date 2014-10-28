# Introduction
Preparation for Red Hat Certified System Administrator (RHCSA) Exam objectives (EX200).

## What you need
This is a difficult one, the answer is it depends. Ihere is very little in this exam that cannot be learnt with nothing but a couple of Virtual Machines. The exception is the control of Virtual Machines and some of the file system work.

The simplest option is to use Oracle VirtualBox. It is free and works on Windows, Linux and OSX. Having said that, personally I use KVM while on Linux.

If you have access to VMware, then brilliant, but not all the free options are suitable.ESXi would require extra hardware so many not work for you, and VMware Player only allows you to run a single VM, it will be fine for some stuff, but not others.

You do not really need a subscription to RHEL. Red Hat are one of the best Open Source companies out there. Not only do they publish the source code, they publish it all as packages that make building your own RHEL relatively trivial. The two main projects that do this are [CentOS](http://www.centos.org) and [Scientific Linux](https://www.scientificlinux.org/). Of the two I tend towards CentOS, not for any particular reason, I just do. Make your choice, but there is no real need to stick with it.

## Assumptions

I am assuming that you are able to perform an install of the base OS. I will also assume that you have created a user which you can call whomever you like. I will however be refering to her as [bob](http://www.youtube.com/watch?v=BLTR8qYWJbQ). Unless stated otherwise, I will assume that all commands are run as this user. This means that any commands that need *root* privileges will be prefaced with `sudo`.

The sylabus does not at the time of writing include managing the firewall, not SELinux. However I personally feel these should never be disabled, so as we go through the configuration of services I'll be including how to configure these when necessary. RHEL7 introduced `firewalld` and `firewall-cmd` for managing th `iptables`. As this is the way forward, I will be concentrating on that.
