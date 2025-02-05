---
layout: page
title: FAQ - Client

---

* Do not remove this line (it will not be displayed)
{:toc}

### The client shows a newer version. Why didn't it notify me of an update?

Assuming you have update notifications switched on (in Preferences) this
probably means the newer version is not *recommended* for your device.

In the list of versions in the client, the *recommended version* is
identified by a '\*'. This is the version which is closest to the
*current version* &ndash; the version that the developers of the
application publish to Google Play or their website, or tag in their
source code repository. There may be newer versions than this in the
list &ndash; they could be, for example, test or beta versions. You can
install these, but update notifications are not shown because the
Version Code (Android's scheme for version numbering) is greater than
the _CurrentVersionCode_.

For third-party repositories, it may also be the case that the
maintainers neglected to update the current version in their
repository's metadata.


### Why does F-Droid need these permissions?

F-Droid is an app store, that means it is already entirely responsible
for finding, downloading and installing apps. That means it already has
all permissions, in effect. For example, a malicious app store with no
permissions could modify every app as it installs it, granting itself
all permissions via those modified apps. This is why it is so important
that an app store is Free Software and publicly audited. F-Droid is
both. That said, F-Droid declares the permissions it actually uses so
that it is honest and transparent about what it is doing.

Here are the permissions that F-Droid current uses:

<dl><dt>

Download apps from f-droid.org and other app repositories:

</dt><dd><tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#INTERNET" target="_blank">android.permission.INTERNET</a></tt></dd><dt>

Start itself automatically at boot time so that it can receive updates:

</dt><dd><tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#RECEIVE_BOOT_COMPLETED" target="_blank">android.permission.RECEIVE_BOOT_COMPLETED</a></tt></dd><dt>

For the nearby service to get current Wi-Fi status, and prompt the user to enable Wi-Fi when swapping:

</dt><dd><tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#ACCESS_COARSE_LOCATION" target="_blank">android.permission.ACCESS_COARSE_LOCATION</a></tt><br/>
<tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#ACCESS_NETWORK_STATE" target="_blank">android.permission.ACCESS_NETWORK_STATE</a></tt><br/>
<tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#CHANGE_NETWORK_STATE" target="_blank">android.permission.CHANGE_NETWORK_STATE</a></tt><br/>
<tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#CHANGE_WIFI_MULTICAST_STATE" target="_blank">android.permission.CHANGE_WIFI_MULTICAST_STATE</a></tt><br/>
<tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#CHANGE_WIFI_STATE" target="_blank">android.permission.CHANGE_WIFI_STATE</a></tt><br/>
<tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#ACCESS_WIFI_STATE" target="_blank">android.permission.ACCESS_WIFI_STATE</a></tt></dd><dt>

For the nearby service to see the Bluetooth state, and prompt the user to enable Bluetooth when swapping:

</dt><dd><tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#BLUETOOTH" target="_blank">android.permission.BLUETOOTH</a></tt><br/>
<tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#BLUETOOTH_ADMIN" target="_blank">android.permission.BLUETOOTH_ADMIN</a></tt><br/>
<tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#BLUETOOTH_CONNECT" target="_blank">android.permission.BLUETOOTH_CONNECT</a></tt></dd><dt>

Exchange repository information via the Repo Details screen, and to optionally assist nearby swap connection:

</dt><dd><tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#NFC" target="_blank">android.permission.NFC</a></tt></dd><dt>

Allow the user to enable Wi-Fi AP Hotspot mode from the nearby service:

</dt><dd><tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#WRITE_SETTINGS" target="_blank">android.permission.WRITE_SETTINGS</a></tt></dd><dt>

Allows the nearby service to stay running as long as the user leaves it running:

</dt><dd><tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#WAKE_LOCK" target="_blank">android.permission.WAKE_LOCK</a></tt></dd><dt>

Find and use compatible repositories and mirrors on external storage:

</dt><dd><tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#READ_EXTERNAL_STORAGE" target="_blank">android.permission.READ_EXTERNAL_STORAGE</a></tt><br/>
<tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#MANAGE_EXTERNAL_STORAGE" target="_blank">android.permission.MANAGE_EXTERNAL_STORAGE</a></tt></dd><dt>

Detect when a USB thumb drive has been inserted, so it can be scanned to find compatible repositories and mirrors:

</dt><dd><tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#USB_PERMISSION" target="_blank">android.permission.USB_PERMISSION</a></tt></dd><dt>

Temporarily store and use downloaded files on external storage:

</dt><dd><tt><a href="https://developer.android.com/reference/android/Manifest.permission.html#WRITE_EXTERNAL_STORAGE" target="_blank">android.permission.WRITE_EXTERNAL_STORAGE</a></tt></dd></dl>

F-Droid [Privileged Extension](https://gitlab.com/fdroid/privileged-extension/) is also relevant here, although it falls outside of the Android system of declaring permissions. Privileged Extension is installed with [`priv-app`](https://source.android.com/docs/core/permissions/perms-allowlist) permissions, which gives F-Droid system-level access privileges to Android. The use of Privileged Extension improves security by allowing automatic app updates as well as letting the user leave the "Unknown Sources" setting off. Privileged Extension is designed on the principals of "least privilege", so that elevated powers are only granted where they are absolutely needed, and those powers are limited as much as possible.  In order to make it possible outside reviewers to confirm that, we have made Privileged Extension as simple and small as possible.


### What is expert mode?

Enabling the 'Expert Mode' setting in Preferences will make the client
display additional information which is probably not useful to most
people. This includes things like package IDs and signature hashes. Some
extra configuration options also appear.


### I can download apps, but then "Install" is disabled. Why?

Some users have apps such as Twilight installed, which draw directly to
the screen regardless of what app is shown. For security reasons,
Android wisely doesn't allow apps to be installed when such apps are
running. If it did, then people could create apps that draw a fake
"Install" button over the top of the real one, resulting in users
installing unwanted apps. The solution is to disable such apps before
installing via F-Droid.

See [Issue 151](https://gitlab.com/fdroid/fdroidclient/issues/151) or
[this Google+
comment](https://plus.google.com/116713673773180618201/posts/UvW3tgSgdUp)
for more details.


### Why doesn't the client show the number of installs/downloads for each app?

To show how many people had installed an app, we would have to be spying
on them - in other words, keeping track of what apps people install and
uninstall on their devices, and sending that data back to ourselves. We
don't do that, and we're not going to do it.

Theoretically, the number of downloads is available via our web server
logs. However, this would be a meaningless figure because:

1.  I might download an app, and decide not to install it
2.  I might download and install it, then uninstall it immediately
    because I don't like it
3.  I might download my app 1,000,000 times to make it look popular

Additionally, on a technical level, we don't even track that
information. While the back-end server does track hits on each APK,
these are actually served up by multiple front-end servers that cache.
This means one counted hit could represent one download, or a million.
Theoretically we could resolve this, but we are not interested enough to
do so.

Finally, even assuming any of this information were available, what does
it actually mean? Are you going to use an app just because lots of
others do, or ignore it because few others have discovered it yet? Is
this a sensible way to decide whether something is useful to you or not?
Perhaps you should just try it.

### How can I send or setup the F-Droid app using NFC or Android Beam?

Starting with v1.20, the F-Droid client does not support these features anymore as the underlying code has been removed from the Android 14 SDK after being deprecated since Android 10. More info [here](https://www.xda-developers.com/android-beam-permanent-removal-android-14/).

### How can I send apps via Bluetooth or WiFi?

This is done using the 'Nearby' Tab in F-Droid (previously called 'Swap').
See [here](../../tutorials/swap) for a walkthrough.

### What is the security model that F-Droid uses?

The F-Droid security model started out with HTTPS connections and signed
metadata. It has been evolving, inspired by [Debian](https://wiki.debian.org/SecureApt), [The Update
Framework](https://github.com/theupdateframework/tuf/blob/develop/docs/tuf-spec.txt),
and other things. You can read about details here: [Security Model](../Security_Model).
