---
layout: docs
title: Debian packages
next_section: community
permalink: /docs/packages-debian/
---

Third-party packages for Debian Wheezy are available for amd64, i686,
arm7/Beaglebone and arm6/Raspberry Pi.

## Quick start

Decide which type of realtime kernel you want: for i686 and amd64,
your options are RT-PREEMPT, Xenomai, or RTAI. For arm7/Beaglebone and
arm6/Raspberry Pi, Xenomai is the only supported realtime kernel.

The RT-PREEMPT realtime kernel comes from the stock wheezy package
stream. Xenomai is a custom kernel with lower latency;
both are fine for applications with hardware step generation or plain
servo configs. RTAI only makes sense for high-rate software step
generation and dumb hardware (parallel port),
at the expense of signficantly higher maintainence
(RT-PREEMPT and Xenomai installs have no significant kernel
dependencies; RTAI installations only run with the kernel the package
was built for).

Installation instructions can be found in the [Machinekit documentation][1]

[1]:  https://github.com/machinekit/machinekit-docs/blob/master/machinekit-documentation/getting-started/getting-started-platform.asciidoc
