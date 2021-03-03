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

Please send patches as merge requests on the GitLab repository:
https://gitlab.freedesktop.org/libevdev/evtest
