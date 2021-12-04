# ArcDVI VIDC adapter PCBs
30 November 2021


Two PCBs used in the [ArcDVI](https://github.com/evansm7/ArcDVI) project.

These PCBs (#1 and #2) both perform the task of physical interfacing to an Acorn Archimedes VIDC chip, but for different machines.  PCB #1 is an interposer for VIDC-socketed machines (such as A440), which plugs into the VIDC socket and carries a socket for the VIDC.  PCB #2 uses an upturned through-hole PLCC socket to clip around a soldered VIDC (in machines such as A3000).

[vidc_interposer1 schematic](doc/vidc_interposer1.pdf), [vidc_interposer1 board](doc/vidc_interposer1_brd.pdf), [vidc_interposer2 schematic](doc/vidc_interposer2-PTH.pdf),
[vidc_interposer2 board](doc/vidc_interposer2-PTH_brd.pdf)

It was originally hoped that PCB #1 could be used on an A3000 too, with an SMT PLCC socket on the bottom (and nothing mounted on the top).  Those sockets are shallow, and the board level is then too low to clear surrounding components.  (Note there are two odd holes in the board; this was to clear some jumper headers.  These were unnecessarily carried into PCB #2's layout too.  In short, neither board needs these holes anymore.)

A separate project (TBD) is recreating PLCC socket-to-socket interface "blocks", enabling a PLCC socket (rather than plug) to be used on the underside of board #1.

The PCBs are designed in Eagle.

Copyright 2021 Matt Evans

CC BY-SA 3.0