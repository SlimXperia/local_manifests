Start With
============
$ repo init -u git://github.com/SlimRoms/platform_manifest.git -b jb4.2

then

Slimbean for SEMC 2011 devices
==============================
Local manifest needed to build slimbean for the Sony Ericsson 2011 phone line.

Instructions:
==============
Copy roomservice.xml into .repo/local_manifests folder in your slim bean tree

$ repo sync

vendorsetup.sh
===============
Add your device name in vendorsetup.sh

ex:- "add_lunch_combo slim_haida-userdebug"

Remove it before repo sync

after sync add it again 

Build
=======
. build/envsetup.sh

lunch

mka bacon -j# (# =number of core in your cpu)
