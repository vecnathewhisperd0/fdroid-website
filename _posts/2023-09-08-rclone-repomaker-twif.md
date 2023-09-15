---
layout: post
title: "TWIF is back and Rclone support in Fdroidserver and Repomaker"
author: "paulali"
authorWebsite: "https://pmmyr.me"
---

### TWIF is back!
TWIF is back or rather almost.

We have been looking at reviving TWIF for the longest time. Now it is 
almost here. We'd like to hear from you.
Post your updates or news that you'd like the F-Droid community to know
about on the [New TWIF Thread] (https://forum.f-droid.org/t/new-twif-submission-thread/23546)
before Thursday 0000 UTC.

Everyone is Welcome!


### Rclone support in Fdroidserver and Repomaker
[Rclone] (https://rclone.org/) has been dubbed "Rsync for cloud storage",
"The Swiss army knife of cloud storage" and "Technology indistinguishable
from magic" by its users. It is a command-line program that is used to
interact with over [70 cloud services] (https://rclone.org/#providers)
and more in the future. This opens up a whole new world of possibilities 
to users of [Fdroidserver] (https://gitlab.com/fdroid/fdroidserver) in that
they can now host their repositories wherever they deem fit as long as it
is supported by Rclone.

To test Rclone support in Fdroidserver, you can install all the other 
server tools apart from Fdroidserver as explained [here] 
(https://f-droid.org/docs/Installing_the_Server_and_Repo_Tools/).
Then create a Python virtual environment, activate it then install the
Fdroidserver branch with Rclone support with `pip` as
`pip3 install git+https://gitlab.com/pmmayero/fdroidserver.git@switching-s3cmd-for-rclone`
You can also contribute your thoughts on this feature on Gitlab 
[here] (https://gitlab.com/fdroid/fdroidserver/-/merge_requests/1095)

With Rclone support on Fdroidserver looking promising, we are hard at
work incorporating Rclone into [Repomaker] (https://f-droid.org/repomaker/) .
We intend to ensure that Repomaker users have the same options as their
Fdroidserver counterparts.We promise to have a testable Merge Request up soon.
Please be patient.