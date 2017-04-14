---
layout: page
title: Building a Signing Server

---

* Android keys need to be kept safe for the entire life of the app!
* Same goes for F-Droid repo signing keys

* Debian/stretch
* reproducible-builds




## HSM+network

* a super basic PC works best for this

## regular files + USB thumb drives
* since the machine is offline, the extra work of using an HSM is not as important, but it can't hurt to include
* apt-offline
  * unfortunately, it does not work with HTTPS repos unless you are using python 2.7.10 or newer
  * the threat should be less, since it is the downloading machine that interacts via HTTP, not the offline machine

* a laptop is the best for this
  * can be any laptop really, it'll be offline
  * for "full paranoid", go with a chromebook, wipe, reproducibly build coreboot, install Debian
  * buy it off the shelf with cash, who knows what happens in shipping
  * one nice thing about devices without ethernet: its easy to disable the wifi hardware:
  https://www.chromium.org/chromium-os/developer-information-for-chrome-os-devices/acer-c720-chromebook
Sources:
   This device uses a proprietary "binary blob" wifi driver, so that means it is not included in Debian since it is not free software.  In this case, this is actually a feature!  Since we're aiming to keep this machine always offline, its nice to run an install process that cannot enable the networking!


* http://www.devops-blog.net/koji/gpg-signing-rpms-with-sigul-signing-server-koji-integration




Signing Environment
The signing environment must be physically secure. Otherwise, there is no way to prevent smart cards or HSMs from being lost or used to sign inappropriate content. The value and availability requirements of the code-signing infrastructure dictate the physical and logical barriers that must be implemented. For example, for a low-throughput infrastructure it may be sufficient to keep an HSM in a locked room that is accessible to only a limited set of individuals. In contrast, a high-throughput production infrastructure may require a high-security data center.
This paper does not attempt to provide a comprehensive description of how to physically secure a code-signing environment. In general, Microsoft recommends that software publishers apply the principles of defense-in-depth by using multiple security techniques for different layers of their code-signing system. Organizations should consider the following physical security best practices:
Access controls such as locks, keycard cards, or biometrics to restrict access to the code-signing infrastructure
Restricted physical access to HSMs or smart cards
Security cameras
Onsite security guards
Visitor logging
A tools-resistant server safe for online code-signing servers
Logical and physical segregation of the code-signing infrastructure from the production network
Periodic audits of the code-signing infrastructure to ensure compliance with documented practices and design

For non-networked signing services, the signing computer or smart card should be kept offline in a tool-resistant safe when it is not in use. The following procedures are highly recommended for networked code-signing systems:
Keep the signing service behind a firewall or on a separate network. Consider Microsoft Internet Security and Acceleration Server or Server and Domain Isolation with IPSec.
Deploy network authentication and integrity protocols as part of the submission and approval process. Password authentication is generally not recommended. Instead, consider certificate-based authentication that uses certificates that are issued from an internal CA or domain authentication that uses Kerberos. IPSec with mutual authentication is also a viable option.
Consider using a separate drop-off-and-pick-up server as an intermediary between the corporate and signing service networks.
Consider deploying network intrusion-detection systems to detect network-based hacking attempts.
