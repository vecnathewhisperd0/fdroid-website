---
layout: post
title: "TWIF 34: F-Droid is a Planet"
edition: 34
author: "Coffee"
authorWebsite: "https://open.source.coffee"
fdroid: '<em style="padding: 0.15em 0.5em 0.10em; margin-right: 0.1ex; border-style: solid; border-width: medium; border-radius: 1em; color: #0d47a1; font-style: normal; font-weight: bold;">F-Droid</em>'
featuredv1: '<em style="padding: 0.15em 0.5em 0.10em; margin-right: 0.5ex; box-shadow: 0.1em 0.05em 0.1em rgba(0, 0, 0, 0.3); border-radius: 1em; color: black; background: linear-gradient(orange, yellow);">Featured</em>'
featured: '<em style="padding: 0.15em 0.5em 0.10em; margin-right: 0.1ex; border-style: solid; border-width: medium; border-radius: 1em; color: orange; font-style: normal; font-weight: bold;">Featured</em>'
major: '<em style="padding: 0.15em 0.5em 0.10em; margin-right: 0.1ex; border-style: solid; border-width: medium; border-radius: 1em; color: #8ab000; font-style: normal; font-weight: bold;">Major</em>'
number_of_added_apps: 3
number_of_updated_apps: 59
mastodonAccount: "**[@fdroidorg@mastodon.technology](https://mastodon.technology/@fdroidorg)**"
twifTag: "**[#TWIF](https://mastodon.technology/tags/twif)**"
twifThread: "[TWIF submission thread](https://forum.f-droid.org/t/twif-submission-thread)"
matrixRoom: "[#fdroid:f-droid.org](https://matrix.to/#/#fdroid:f-droid.org)"
telegramRoom: "https://t.me/joinchat/AlRQekvjWDTuQrCgMYSNVA"
forum: "https://forum.f-droid.org"
---

This Week In F-Droid {{ page.edition }}, Week {{ page.date | date: "%V, %G" }} <a href="{{ site.baseurl }}/feed.xml"><img src="{{ site.baseurl }}/assets/Feed-icon-16x16.png" alt="Feed"></a>

In this edition: Planet F-Droid now exists, call for submissions for Planet F-Droid and first article of Izzy's F-Droid series available in English.
There are **{{ page.number_of_added_apps }}** new and **{{ page.number_of_updated_apps }}** updated apps.

<!--more-->

**[F-Droid](https://f-droid.org/)** is a [repository](https://f-droid.org/packages/) of verified [free and open source](https://en.wikipedia.org/wiki/Free_and_open-source_software) Android apps, a **[client](https://f-droid.org/app/org.fdroid.fdroid)** to access it, as well as a whole "app store kit", providing all the tools needed to set up and run an app store. It is a community-run free software project developed by a wide range of contributors. This is their story this past week.

### Planet F-Droid now exists

F-Droid now has [its own planet](https://fdroid.gitlab.io/planet/), thanks to the hard work of **[@vanitasvitae](https://gitlab.com/vanitasvitae)**, who single-handedly set it all up! A so-called "planet" site aggregates the blogs of community members (see [http://planet.fsfe.org](http://planet.fsfe.org) or [https://planet.jabber.org](https://planet.jabber.org) as examples). And if you've been secretly following along via [the forum](https://forum.f-droid.org/t/planet-f-droid-org-feed-aggregator-for-android-dev-related-blogs/4481), Planet F-Droid now also has [the blog of Gregor Santner](https://gsantner.net/), of **[Markor](https://f-droid.org/app/net.gsantner.markor)**, **[MemeTastic](https://f-droid.org/app/io.github.gsantner.memetastic)** and **[dandelion\*](https://f-droid.org/app/com.github.dfa.diaspora_android)** fame.

### Call for submissions for Planet F-Droid

Hello FOSS Android enthusiasts and project leads! Do you want your FOSS and Android related blog to be included in [Planet F-Droid](https://fdroid.gitlab.io/planet/)? Please have a look at the Planet's [inclusion rules](https://gitlab.com/fdroid/planet/wikis/inclusion-rules), or [read more about it](https://gitlab.com/fdroid/planet/wikis/Planet-F-Droid).

### First article of Izzy's F-Droid series available in English

**[@Izzy](https://forum.f-droid.org/u/izzy)** [writes](https://mastodon.technology/users/IzzyOnDroid/statuses/101210904206926714):

Happy Chanukka, happy 2nd advent – and here comes a little present: I've just put the first article of my F-Droid series online. "F-Droid: The privacy-friendly alternative to Google Play Store" can be found at [https://android.izzysoft.de/articles/named/fdroid-intro-1](https://forum.f-droid.org/t/planet-f-droid-org-feed-aggregator-for-android-dev-related-blogs/4481).

Die deutsche Fassung verzögert sich noch ein wenig. Wer es nicht abwarten kann, kauft sich die c't 25, der ich (nach Vereinbarung mit Heise) ein paar Wochen Vorsprung geben muss. 😉

### New apps

* **[DeltaCamera](https://f-droid.org/app/de.uwepost.android.deltacam)**: Record movement (deltas) in one single image.
* **[AnLinux](https://f-droid.org/app/exa.lnx.a)**: Run linux on android without root access.
* **[/d/gapps](https://f-droid.org/app/org.droidtr.deletegapps)**: Delete/disable gapps.

### Updated apps

In total, **{{ page.number_of_updated_apps }}** apps were updated this week. Here are the highlights:

* **[Music Player GO](https://f-droid.org/app/com.iven.musicplayergo)** was [updated](https://github.com/enricocid/Music-Player-GO/releases) from 3.5.0.2 to 3.5.2.1 with code cleaning and simplifications, new scroller with touching the edge of the screen, minor changes to UI and layout, a new Turkish translation, smaller APK, and assorted bugfixes.

* {{ page.featured }} **[Mastalab](https://f-droid.org/app/fr.gouv.etalab.mastodon)** was [updated](https://gitlab.com/tom79/mastalab/tags) from 1.36.0 to 1.39.0 and now has an art timeline! The buttons for boosting or favoriting are now animated, "create toot" button is hidden while scrolling, there is support for scheduling _boosts_ (toots could already be scheduled), and many bugs were fixed. Oh, and it should now have textual descriptions for everything, for visually impaired users.

* {{ page.featured }} **[Markor](https://f-droid.org/app/net.gsantner.markor)** comes with lots of changes in 1.5.0. I could write a summary, but you should really just check the [release blog post](https://gsantner.net/blog/2018/12/09/markor-release-v1.5.html) which explains everything in pictures! (And also in words.)

* **[Open Contacts](https://f-droid.org/app/opencontacts.open.com.opencontacts)** was [updated](https://gitlab.com/sultanahamer/OpenContacts/blob/HEAD/CHANGELOG) from 7.0 to 9.0, featuring a dark theme, support for phone numbers with symbols, delete all contacts, several UI and UX improvements and bugfixes, including an important fix for a crash in Android 8 (Oreo). **Please export and reimport all your contacts** in order for search to work. Apologies, but it's only a one-time thing.

* **[AndStatus](https://f-droid.org/app/org.andstatus.app)** [updated](http://andstatus.org/changelog.html) to 45.01, adding the "unread notifications" timeline. It also has improved handling of HTML content.

* **[SimpleEmail](https://f-droid.org/app/org.dystopia.email)** 1.3.0 brings a better layout for the message list, refresh message list, and moves the color picker account outside of advanced.

### Removed apps

* **[Iven News Reader](https://f-droid.org/wiki/page/com.iven.lfflfeedreader)** was moved to the archive because the app has been marked as "deprecated" by its author.

### Tips and Feedback

Do you have important app updates we should write about? Send in your tips via [Mastodon](https://joinmastodon.org)! Send them to {{ page.mastodonAccount }} and remember to tag with {{ page.twifTag }}. Or use the {{ page.twifThread }} on the forum. The deadline to the next TWIF is **Thursday** 12:00 UTC.

General feedback can also be sent via Mastodon, or, if you'd like to have a live chat, you can find us in **#fdroid** on [Freenode](https://freenode.net), on Matrix via {{ page.matrixRoom }} or on [Telegram]({{ page.telegramRoom }}). All of these spaces are bridged together, so the choice is yours. You can also join us on the **[forum]({{ page.forum }})**.
