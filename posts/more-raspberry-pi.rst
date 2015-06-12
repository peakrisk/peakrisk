.. title: More raspberry pi
.. slug: more-raspberry-pi
.. date: 2015-06-10 18:38:29 UTC
.. tags: raspberry pi, linux
.. category: 
.. link: 
.. description: 
.. type: text

I am going to be doing an introduction to free software and linux for
this year's `Technology Leadership Forum`_ students.

The plan is to have the students use raspberry pi's to learn about the
linux platform.

I have a bunch of the new raspberry pi 2's and have been experimenting
with different linux distributions on these pi's.

I was going to write up my experiences, but Swapnil Bhartiya has
kindly `blogged`_ about his own experiences with Arch, Raspbian and
Ubuntu Snappy Core.  His conclusions were similar to my own.

Arch
====

I have been using `Arch Linux`_ a little of late and like many things
about Arch and `The Arch Way`_.

First of all, the Arch wiki has excellent documentation.  This is
critical to its success, since it does many things a little
differently to the larger linux distributions.

An initial Arch install will not install much beyond the bare
essentials to get you up and running.  This does mean it can take a
little while to get a new system just how you want it, but has the
advantage you do not end up with hundreds of packages installed which
you have little idea what they do.  For the security conscious this is
a definite plus.

One feature I love is that their are no *dev* packages.  Anyone who
has tried using any of the main linux distributions and is in the
habit of compiling code on those systems will have run into the
situation where code fails to build due to missing C header files.

In the major distributions these header files are in separate *dev*
packages.  The philosophy is that most people are not compiling code
on these machines so do not need the header files.  This choice is
fine until a new user decides to try compiling some code and then is
hit by the missing header file issue.  Just another obstacle put in
the way of potential new developers.

In contrast, Arch argues that these header files are generally tiny
and including them in the main package adds little overhead and saves
a lot of time for anyone doing development.   It would be good if more
distros made this switch.

Using Arch will present some challenges to a new user, but given the
excellent state of the documentation it is also an excellent way to
gain a thorough understanding of how everything works.

Raspbian
========

Raspbian appears to be the most widely used distribution on the
raspberry pi.   It is based on the Debian and has over 35,000 packages
available.

Since I have mostly used Debian based distributions this seems a good
place to start.

Trying different distros can get a little time consuming, between
downloading images and copying them onto SD cards.  Further, different
images are needed for the older pi's and the pi 2.

The simplest way to get a Raspian system up and running is to
`download`_ the raspian image from raspberrypi.org.

To install just copy to the SD card device using dd::

  dd if=raspian_image_you_downloaded.img of=/dev/SDCARD

Finding the device for your SD card can be tricky. *lsblk* shows you
all the block devices and with luck your SD card will be there.

On my Ubuntu system it is /dev/mmblk0, on an Arch machine it showed up
as /dev/sdb.  You can usually figure things out using the SIZE of the
device.

Note also that you want the block with TYPE disk, not any of the
partitions it might have.

Raspbain installer
==================

Another approach is to use this `Raspbian installer`_.   One clear
advantage is that it is a small download, a mere 11MB and a small copy
onto your SD card.

You then just plug it into the pi, turn on the pi with a wired network
connection and the install happens by magic.  It takes 20 minutes or
so, with a reasonable internet connection.

Other advantages include:

* you use the same installer for the original pi's and the pi 2.

* the installer installs the latest packages from the release
  (currently wheezy) that you choose.
  
* you can customise the installer to include additional packages and a
  number of other customisations.

The down side is that the base install comes without a GUI
environment.  Depending on what you intend to do with the pi this may
not be a problem.

I am going to experiment with customising the installer to see if I
can get it to install lxde, emacs, git and some other goodies I like
to have around on my systems.


.. include:: posts/references.rst

.. _download: https://www.raspberrypi.org/downloads/
.. _Arch Linux: https://www.archlinux.org/

.. _Raspbian installer: https://github.com/debian-pi/raspbian-ua-netinst

.. _The Arch Way: https://wiki.archlinux.org/index.php/The_Arch_Way
.. _blogged: `Getting started with the pi 2`_

