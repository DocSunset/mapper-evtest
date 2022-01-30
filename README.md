WARNING: this program provides libmapper bindings to linux evdev.  Anyone
connecting to these libmapper devices can see all your interactions with the
device, regardless of whether this program is in the foreground or running in a
background process.  Be careful not to expose sensitive information such as
passwords if you expose your keyboard and mouse to the network!

evtest — Kernel input device debugging
======================================

evtest is a tool to print evdev kernel events. It reads directly from the
kernel device and prints a device description and the events with the value
and the symbolic name.

Usage:

    evtest /dev/input/event0

Note: in most cases evtest needs to run as root to be able to read the
devices.

For more information, see the evtest(1) man page.

Development
==========

This fork of evtest is maintained by Travis West on github: https://github.com/docsunset/mapper-evtest
