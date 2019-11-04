---
layout: post
title: "Announcing GitLab CI Emulator Images"
author: "eighthave"
---

GitLab CI (Continuous Integration) has become an essential part of the
F-Droid community processes.  It is free software, built on open
standards, and works well.  The last piece that was missing from our
testing ecosystem was a reliable way to run tests in actual Android
emulators.  Now, the standard 
[_fdroidclient_ CI setup]()
provides

* works without KVM or any extra privileges
* works on the default gitlab.com runners
* also uses KVM when available
*

Before, we were limited only using _armeabi_ emulators, which are run
really slow.
