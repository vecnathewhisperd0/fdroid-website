---
layout: post
title: "Contributor Highlights"
author: "paulali"
---


### TWIF generated on Thursday, 26 Oct 2023 ,Week 43


#### F-Droid core
**[F-Droid](https://f-droid.org/packages/org.fdroid.fdroid)** and **[F-Droid Basic](https://f-droid.org/packages/org.fdroid.basic)** were updated from 1.18.0 to 1.19.0-alpha0, now with support for automatic background updates on Android 12+ as announced [last week](https://f-droid.org/2023/10/19/twif-client-alpha-kde-removal-by-google.html). _Note that this is still in `beta` so brave users need to install this manually (enable Beta updates for the app or from Client expert settings)._


#### Community News

[@Licaon_Kter](https://gitlab.com/licaon-kter) comments:

**[Aurora Store](https://f-droid.org/packages/com.aurora.store)** was updated from 4.3.3 to 4.3.5 fixing an important installation issue so users are advised to update.

**[Conversations](https://f-droid.org/packages/eu.siacs.conversations)** was updated from 2.12.11+free to 2.12.12-beta.2+free adding experimental support for Private DNS (DNS over TLS), themed icon on Android 13+ and many other fixes. _Note that this is still in `beta` so brave users need to install this manually (enable Beta updates for the app or from Client expert settings)._ The missing website description will be fixed in the next few days.

**[Linphone - open source SIP client](https://f-droid.org/packages/org.linphone)** was updated from 5.1.3 to 5.1.4 and now supports the narrow-band vocoder-based audio data compression algorithm G.729.

**[Prav](https://f-droid.org/packages/app.prav.client)** is live in F-Droid! It's a fork of [Quicksy](https://f-droid.org/packages/im.quicksy.client/) keeping the same easy onboarding for new XMPP users and phone number based automatic contact discovery. [Prav is based in India](https://prav.app/) and is backed by a cooperative society. Being an XMPP client it means it can communicate with XMPP users on servers all around the world.


[@linsui](https://gitlab.com/linsui) comments:

I want to highlight some updates of this week:

**[Image Toolbox](https://f-droid.org/packages/ru.tech.imageresizershrinker/)** is finally updated again. Since 2.1.3 [we can't build the APK reproducibly](https://github.com/T8RIN/ImageToolbox/discussions/151). Then some prebuilt libs are added which introduces more problems. Thanks to the effort of [@Licaon_Kter](https://gitlab.com/licaon-kter) and [@T8RIN](https://github.com/T8RIN) those binaries are cleaned up and the APK is reproducible again after 4 months.

**[Kubenav](https://f-droid.org/packages/io.kubenav.kubenav/)** is rewriten in Flutter and Go since 4.0.0. This broke the update checker and we only noticed that recently. [@linsui](https://gitlab.com/linsui) [added](https://gitlab.com/fdroid/fdroiddata/-/merge_requests/13850) [v4.2.3](https://github.com/kubenav/kubenav/releases/tag/v4.2.3) and patched out some new non-free deps. It should be updated automatically in the future.

**[Sayboard](https://f-droid.org/packages/com.elishaazaria.sayboard/)**, a voice IME, is in F-Droid now. We have many open source IME but none of them have voice input support. Now we have an open source voice IME based on Vosk.Yay!!!

**[Standard Notes](https://f-droid.org/packages/com.standardnotes/)** is back! The license of Standard Notes was [changed](https://github.com/standardnotes/app/commit/9e908f344c6a15c961310b6b57e1c56032ac50df) from AGPL3 to BY-NC-SA 4.0 which is not an FOSS license. After it was [reported](https://gitlab.com/fdroid/fdroiddata/-/issues/3069), we [disabled affected versions and don't update it anymore](https://gitlab.com/fdroid/fdroiddata/-/commit/ee585f7f512e78518556c66f44dbb398a5db2475). Recently, the change was [reverted](https://github.com/standardnotes/app/commit/d254e1c4e34793c23b0c62c24bb239dda5187365) so Standard Notes is FOSS again! More details can be found [here](https://github.com/standardnotes/forum/discussions/3196). [@proletarius101](https://gitlab.com/proletarius101) [re-enabled](https://gitlab.com/fdroid/fdroiddata/-/merge_requests/13878) with an update.

**[TIDY Text-to-Image Discovery](https://f-droid.org/packages/com.slavabarkov.tidy)**, a local image search tool, is in F-Droid now. It brings the power of AI to your phone, running totally offline!


#### Removed Apps
##### 5 apps were removed
**Carfoin**'s API no longer works so [the developer asked](https://gitlab.com/fdroid/rfp/-/issues/2228#note_1613219015) for it to be removed. 

**Infinity for Reddit** can no longer connect to the website ([#3098](https://gitlab.com/fdroid/fdroiddata/-/issues/3098))

**RadioBeacon** and **Radiocells.org UnifiedNlp Backend** used a backend database that is no longer accessible ([#3102](https://gitlab.com/fdroid/fdroiddata/-/issues/3102))

**WireGuard**'s in-app updater makes it no longer eligible for [inclusion](https://f-droid.org/docs/Inclusion_Policy/) in F-Droid. WireGuard users can get updates directly from upstream or switch to one of the alternatives.


#### Newly Added Apps
##### 17 more apps were newly added
* **[8-Bit Wonders](https://f-droid.org/packages/de.rainerhock.eightbitwonders)**
* **[Ansible Sempahore Client](https://f-droid.org/packages/org.gsmlg.semaphore)**
* **[Audile](https://f-droid.org/packages/com.mrsep.musicrecognizer)**
* **[Candle](https://f-droid.org/packages/com.elasticrock.candle)**
* **[Friend Alert](https://f-droid.org/packages/xyz.crucitti.friendalert)**
* **[JS-Dict](https://f-droid.org/packages/io.github.petlyh.jsdict)**
* **[LibreRandonaut](https://f-droid.org/packages/com.github.librerandonaut.librerandonaut)**
* **[NanoLedger](https://f-droid.org/packages/be.chvp.nanoledger)**
* **[Oinkoin](https://f-droid.org/packages/com.github.emavgl.piggybankpro)**
* **[OpenAthena™ for Android](https://f-droid.org/packages/com.openathena)**
* **[Quran 16 Line - Quran Revision Helper](https://f-droid.org/packages/com.wqar.quran_mem_helper)**
* **[SerialPipe](https://f-droid.org/packages/io.github.wh201906.serialpipe)**
* **[SilverDict](https://f-droid.org/packages/com.gmail.blandilyte.silverdict)**
* **[SpMp](https://f-droid.org/packages/com.toasterofbread.spmp)**
* **[TimePlanner](https://f-droid.org/packages/ru.aleshin.timeplanner)**
* **[Voyager for Lemmy](https://f-droid.org/packages/app.vger.voyager)**
* **[huggingAssist](https://f-droid.org/packages/org.woheller69.hugassist)**


#### Downgraded Apps
##### 2 apps were downgraded
**[Podverse](https://f-droid.org/packages/com.podverse.fdroid)** was downgraded from 4.14.0 to 4.13.9 as the new version was crashing.

**[Shattered Pixel Dungeon](https://f-droid.org/packages/com.shatteredpixel.shatteredpixeldungeon)** was updated to 2.2.0 then downgraded to 2.1.4 as the [new version is crashing](https://gitlab.com/fdroid/fdroiddata/-/issues/3115), please wait for a fixed version 2.2.1.


#### Updated Apps
##### ~163 more apps were updated
* **[8Vim Keyboard](https://f-droid.org/packages/inc.flide.vi8)** was updated from 0.14.0 to 0.16.2
* **[Acode editor - Android code editor](https://f-droid.org/packages/com.foxdebug.acode)** was updated, but uses the same 1.8.7 version naming
* **[AF Weather Widget](https://f-droid.org/packages/net.gitsaibot.af)** was updated from 2.2 to 2.3
* **[AirGuard - AirTag protection](https://f-droid.org/packages/de.seemoo.at_tracking_detection)** was updated from 2.0 to 2.1
* **[Amethyst](https://f-droid.org/packages/com.vitorpamplona.amethyst)** was updated from 0.79.3 to 0.79.12
* **[Androidacy Module Manager](https://f-droid.org/packages/com.fox2code.mmm.fdroid)** was updated from 2.3.3-fdroid to 2.3.4-fdroid
* **[Arcticons Dark](https://f-droid.org/packages/com.donnnno.arcticons)** was updated from 7.3.7 to 7.5.4
* **[Arcticons Light](https://f-droid.org/packages/com.donnnno.arcticons.light)** was updated from 7.3.7 to 7.5.4
* **[Arcticons You](https://f-droid.org/packages/com.donnnno.arcticons.you)** was updated from 7.3.7 to 7.5.4
* **[Audio Share](https://f-droid.org/packages/io.github.mkckr0.audio_share_app)** was updated from 0.0.9 to 0.0.11
* **[Auto Auto-Rotate](https://f-droid.org/packages/com.jarsilio.android.autoautorotate)** was updated from 0.12.2 to 0.12.3
* **[Aves Libre](https://f-droid.org/packages/deckers.thibault.aves.libre)** was updated from 1.9.6 to 1.9.7
* **[Baby Phone](https://f-droid.org/packages/com.serwylo.babyphone)** was updated from 1.1.3 to 1.2.0
* **[Ball2Box](https://f-droid.org/packages/com.simondalvai.ball2box)** was updated from 4.0.0 to 4.0.1
* **[baresip+](https://f-droid.org/packages/com.tutpro.baresip.plus)** was updated from 45.0.0 to 46.1.0
* **[baresip](https://f-droid.org/packages/com.tutpro.baresip)** was updated from 58.0.0 to 59.0.3
* **[Beat Feet](https://f-droid.org/packages/com.serwylo.beatgame)** was updated from 0.15.0 to 0.16.0
* **[Binary Eye](https://f-droid.org/packages/de.markusfisch.android.binaryeye)** was updated from 1.60.3 to 1.61.0
* **[Blitzortung Lightning Monitor](https://f-droid.org/packages/org.blitzortung.android.app)** was updated from 2.1.14 to 2.2.1
* **[blocker](https://f-droid.org/packages/com.merxury.blocker)** was updated from 2.0.2485 to 2.0.2914-fdroid
* **[BOINC](https://f-droid.org/packages/edu.berkeley.boinc)** was updated from 7.22.2 to 7.24.1
* **[Box, Box!](https://f-droid.org/packages/org.brightdv.boxbox)** was updated from 0.6.3 to 0.6.4
* **[Briar](https://f-droid.org/packages/org.briarproject.briar.android)** was updated from 1.5.7 to 1.5.8
* **[Canta](https://f-droid.org/packages/org.samo_lego.canta)** was updated from 1.1.2 to 1.2.0
* **[CatBox](https://f-droid.org/packages/moe.cb4a)** was updated from 1.2.6 to 1.2.7
* **[Chaldea](https://f-droid.org/packages/cc.narumi.chaldea.fdroid)** was updated from 2.4.17 to 2.4.19
* **[Cheogram](https://f-droid.org/packages/com.cheogram.android)** was updated from 2.12.8-2+free to 2.12.8-3+free
* **[Chip Defense](https://f-droid.org/packages/de.chadenas.cpudefense)** was updated from 1.21 to 1.22
* **[ClashMetaForAndroid](https://f-droid.org/packages/com.github.metacubex.clash.meta)** was updated from 2.8.8.Meta-Alpha to 2.8.10.Meta-Alpha
* **[Clipious](https://f-droid.org/packages/com.github.lamarios.clipious)** was updated from 1.16.4 to 1.17.0
* **[Coffee](https://f-droid.org/packages/com.github.muellerma.coffee)** was updated from 2.19 to 2.20
* **[Commons](https://f-droid.org/packages/fr.free.nrw.commons)** was updated from 4.1.0 to 4.2.0
* **[Conversations](https://f-droid.org/packages/eu.siacs.conversations)** was updated from 2.12.11+free to 2.12.12-beta.2+free
* **[Coordinate Joker](https://f-droid.org/packages/com.github.siggel.coordinatejoker)** was updated from 1.3.32 to 1.4.34
* **[Copy SMS Code - OTP Helper](https://f-droid.org/packages/io.github.jd1378.otphelper)** was updated from 1.3.0 to 1.4.0
* **[croc](https://f-droid.org/packages/com.github.howeyc.crocgui)** was updated from 1.10.11 to 1.10.12
* **[Dark Mode Live Wallpaper](https://f-droid.org/packages/com.github.cvzi.darkmodewallpaper)** was updated from 1.6.3 to 1.6.4
* **[Diaguard: Diabetes Diary](https://f-droid.org/packages/com.faltenreich.diaguard)** was updated from 3.11.1 to 3.12.1
* **[Drinkable](https://f-droid.org/packages/com.moimob.drinkable)** was updated from 1.39.0 to 1.41.0
* **[Droid-ify](https://f-droid.org/packages/com.looker.droidify)** was updated from 0.5.9 Patch 1 to 0.5.9 Patch 4
* **[DroidRec](https://f-droid.org/packages/com.yakovlevegor.DroidRec)** was updated from 3.5 to 3.6
* **[droidVNC-NG](https://f-droid.org/packages/net.christianbeier.droidvnc_ng)** was updated from 2.1.3 to 2.1.5
* **[DuckDuckGo Privacy Browser](https://f-droid.org/packages/com.duckduckgo.mobile.android)** was updated from 5.172.2 to 5.174.0
* **[Easy Diary](https://f-droid.org/packages/me.blog.korn123.easydiary)** was updated from 1.4.302.202309180 to 1.4.303.202310160
* **[EinkBro](https://f-droid.org/packages/info.plateaukao.einkbro)** was updated from 10.14.0 to 10.15.0
* **[Endless Sky](https://f-droid.org/packages/com.github.thewierdnut.endless_mobile)** was updated from 0.10.3-38 to 0.10.4-39
* **[ente Authenticator](https://f-droid.org/packages/io.ente.auth)** was updated from 2.0.8 to 2.0.12
* **[ente - encrypted photo storage](https://f-droid.org/packages/io.ente.photos.fdroid)** was updated from 0.7.100 to 0.7.102
* **[Escapepod - Podcast Player](https://f-droid.org/packages/org.y20k.escapepod)** was updated from 1.1.1 to 1.1.2
* **[FairEmail](https://f-droid.org/packages/eu.faircode.email)** was updated from 1.2108 to 1.2113
* **[Fast Draw](https://f-droid.org/packages/peterfajdiga.fastdraw)** was updated from 1.6 to 1.7
* **[FediPhoto-Lineage](https://f-droid.org/packages/com.fediphoto.lineage)** was updated from 7.1 to 7.2
* **[Feeder](https://f-droid.org/packages/com.nononsenseapps.feeder)** was updated from 2.6.6 to 2.6.7-1
* **[Fennec F-Droid](https://f-droid.org/packages/org.mozilla.fennec_fdroid)** was updated from 118.1.0 to 118.2.0
* **[FFUpdater](https://f-droid.org/packages/de.marmaro.krt.ffupdater)** was updated from 78.2.4 to 78.3.0
* **[Flipper Mobile App](https://f-droid.org/packages/com.flipperdevices.app)** was updated from 1.6.4 to 1.6.5
* **[Gallery for PhotoPrism](https://f-droid.org/packages/ua.com.radiokot.photoprism)** was updated from 1.20.0 to 1.20.1
* **[Godot Editor 4](https://f-droid.org/packages/org.godotengine.editor.v4)** was updated from 4.0.1.stable.0 to 4.1.2.stable
* **[Graded - Grade tracker](https://f-droid.org/packages/com.NightDreamGames.Grade.ly)** was updated from 2.4.1 to 2.4.2
* **[GreenStash](https://f-droid.org/packages/com.starry.greenstash)** was updated from 2.7.0 to 2.8.0
* **[Gurgle](https://f-droid.org/packages/org.billthefarmer.gurgle)** was updated from 1.25 to 1.26
* **[Hacki for Hacker News](https://f-droid.org/packages/com.jiaqifeng.hacki)** was updated from 1.9.3 to 2.0.1
* **[Hail](https://f-droid.org/packages/com.aistra.hail)** was updated from 1.5.0 to 1.6.0
* **[HexViewer](https://f-droid.org/packages/fr.ralala.hexviewer)** was updated from 1.46 to 1.48
* **[IITC-CE Mobile](https://f-droid.org/packages/org.exarhteam.iitc_mobile)** was updated from 0.36.1 to 0.37.0
* **[Immich](https://f-droid.org/packages/app.alextran.immich)** was updated from 1.81.0 to 1.82.0
* **[Infomaniak kDrive](https://f-droid.org/packages/com.infomaniak.drive)** was updated from 4.2.30 to 4.2.31
* **[Infomaniak Mail](https://f-droid.org/packages/com.infomaniak.mail)** was updated from 1.0.15 to 1.0.17
* **[Insigno](https://f-droid.org/packages/org.mindshub.insigno)** was updated from 1.4.0 to 1.4.2
* **[Jami](https://f-droid.org/packages/cx.ring)** was updated from 20231006-01 to 20231019-01
* **[jtx Board journals & notes & tasks](https://f-droid.org/packages/at.techbee.jtx)** was updated from 2.06.00.ose to 2.06.01.ose
* **[JustChess](https://f-droid.org/packages/com.alaskalinuxuser.justchess)** was updated from 2.4 to 2.5
* **[Keep Screen On](https://f-droid.org/packages/com.elasticrock.keepscreenon)** was updated from 1.11.0 to 1.12.0
* **[KitchenOwl](https://f-droid.org/packages/com.tombursch.kitchenowl)** was updated from 0.4.12 to 0.4.13
* **[Kotatsu](https://f-droid.org/packages/org.koitharu.kotatsu)** was updated from 6.1.6 to 6.2.2
* **[kubenav](https://f-droid.org/packages/io.kubenav.kubenav)** was updated from 3.9.0 to 4.2.3
* **[Kvaesitso](https://f-droid.org/packages/de.mm20.launcher2.release)** was updated from 1.27.1-fdroid to 1.28.0-fdroid
* **[Kwik EFIS](https://f-droid.org/packages/player.efis.pfd)** was updated from 6.14 to 6.15
* **[LavSeeker](https://f-droid.org/packages/org.woheller69.lavatories)** was updated from 2.1 to 2.2
* **[LibrePass](https://f-droid.org/packages/dev.medzik.librepass.android)** was updated from 1.0.0-alpha04 to 1.0.0-alpha06
* **[LibreTube](https://f-droid.org/packages/com.github.libretube)** was updated from 0.18.1 to 0.19.0
* **[Linwood Butterfly](https://f-droid.org/packages/dev.linwood.butterfly.nightly)** was updated from 2.0.0-beta.9 to 2.0.0-beta.11
* **[Locus](https://f-droid.org/packages/app.myzel394.locus)** was updated from 0.15.1 to 0.15.2
* **[LogFox](https://f-droid.org/packages/com.f0x1d.logfox)** was updated from 1.4.4 to 1.4.6
* **[Massive](https://f-droid.org/packages/com.massive)** was updated from 1.157 to 1.164
* **[Mattermost Beta](https://f-droid.org/packages/com.mattermost.rnbeta)** was updated from 2.8.2 to 2.9.0
* **[MinCal Widget](https://f-droid.org/packages/cat.mvmike.minimalcalendarwidget)** was updated from 2.12.7 to 2.13.0
* **[Minesweeper - Antimine](https://f-droid.org/packages/dev.lucanlm.antimine)** was updated from 17.5.0 F to 17.5.1 F
* **[Miru](https://f-droid.org/packages/miru.miaomint)** was updated from 1.7.1 to 1.7.2
* **[Moonlight Game Streaming](https://f-droid.org/packages/com.limelight)** was updated from 11.0 to 12.0.1
* **[MOROway App](https://f-droid.org/packages/de.moroway.oc)** was updated from 8.1.8 to 9.0.0
* **[MultiVNC](https://f-droid.org/packages/com.coboltforge.dontmind.multivnc)** was updated from 2.1.3 to 2.1.4
* **[MuPDF mini](https://f-droid.org/packages/com.artifex.mupdf.mini.app)** was updated from 1.23.3a to 1.23.4a
* **[MuPDF viewer](https://f-droid.org/packages/com.artifex.mupdf.viewer.app)** was updated from 1.23.3a to 1.23.4a
* **[Muzei](https://f-droid.org/packages/net.nurik.roman.muzei)** was updated from 3.5.0-alpha05 to 3.5.0-rc01
* **[My Leaf](https://f-droid.org/packages/dk.kjeldsen.carwingsflutter)** was updated from 2.3.0 to 2.3.1
* **[Myne: Ebook Downloader](https://f-droid.org/packages/com.starry.myne)** was updated from 1.5.0 to 2.6.0
* **[Nekome](https://f-droid.org/packages/com.chesire.nekome)** was updated from 2.0.5 to 2.1.1
* **[Nextcloud Cookbook](https://f-droid.org/packages/de.lukasneugebauer.nextcloudcookbook)** was updated from 0.13.0 to 0.14.3
* **[Nextcloud Dev](https://f-droid.org/packages/com.nextcloud.android.beta)** was updated from 20231012 to 20231022
* **[Nextcloud Talk](https://f-droid.org/packages/com.nextcloud.talk2)** was updated from 17.1.0 to 17.1.2
* **[Noice: Natural calming noise](https://f-droid.org/packages/com.github.ashutoshgngwr.noice)** was updated from 2.5.3 to 2.5.4
* **[openHAB Beta](https://f-droid.org/packages/org.openhab.habdroid.beta)** was updated from 3.7.6-beta to 3.7.7-beta
* **[Open Stable Diffusion](https://f-droid.org/packages/com.openstablediffusion)** was updated from 1.7 to 1.8
* **[OpenTracks](https://f-droid.org/packages/de.dennisguse.opentracks)** was updated from v4.9.1 to v4.9.3
* **[ownCloud](https://f-droid.org/packages/com.owncloud.android)** was updated from 4.1.0 to 4.1.1
* **[Periodical](https://f-droid.org/packages/de.arnowelzel.android.periodical)** was updated from 1.74 to 1.75
* **[Permission Manager X](https://f-droid.org/packages/com.mirfatif.permissionmanagerx)** was updated from v1.21-fd to v1.23-fd
* **[Phonograph Plus](https://f-droid.org/packages/player.phonograph.plus)** was updated from 1.3.1 to 1.3.2
* **[PianOli](https://f-droid.org/packages/com.nicobrailo.pianoli)** was updated from 1.22 to 1.24
* **[Pineapple Lock Screen (OSS)](https://f-droid.org/packages/net.blumia.pineapple.lockscreen.oss)** was updated from 1.2.3-oss to 1.3.0-oss
* **[PipePipe](https://f-droid.org/packages/InfinityLoop1309.NewPipeEnhanced)** was updated from 3.1.4 to 3.1.5
* **[Pocket Broomball](https://f-droid.org/packages/com.simondalvai.pocketbroomball)** was updated from 5.0.4 to 5.0.5
* **[pretixPRINT](https://f-droid.org/packages/eu.pretix.pretixprint)** was updated from 2.16.1-foss to 2.16.2-foss
* **[QRAlarm](https://f-droid.org/packages/com.sweak.qralarm)** was updated from 1.5.5 to 1.5.6
* **[QuickDic](https://f-droid.org/packages/de.reimardoeffinger.quickdic)** was updated from 5.6.3 to 5.7.1
* **[QuickWeather](https://f-droid.org/packages/com.ominous.quickweather)** was updated from 2.5.4 to 2.5.5
* **[Quote Unquote](https://f-droid.org/packages/com.github.jameshnsears.quoteunquote)** was updated from 4.36.0-fdroid to 4.36.1-fdroid
* **[Radar App](https://f-droid.org/packages/org.radar.app)** was updated from 0.6 to 0.7
* **[Reader for Selfoss](https://f-droid.org/packages/bou.amine.apps.readerforselfossv2.android)** was updated from 123102852-github to 123102961-github
* **[Saber](https://f-droid.org/packages/com.adilhanney.saber)** was updated from 0.16.1 to 0.17.0
* **[Safe Space](https://f-droid.org/packages/org.privacymatters.safespace)** was updated from 1.1.5 to 1.2.0
* **[SCEE](https://f-droid.org/packages/de.westnordost.streetcomplete.expert)** was updated from 53.32 to 54.12
* **[SchildiChat](https://f-droid.org/packages/de.spiritcroc.riotx)** was updated from 1.6.5.sc72 to 1.6.6.sc73
* **[Screenshot Tile (NoRoot)](https://f-droid.org/packages/com.github.cvzi.screenshottile)** was updated from 2.3.7 to 2.5.2
* **[Session F-Droid](https://f-droid.org/packages/network.loki.messenger.fdroid)** was updated from 1.17.3 to 1.17.4
* **[Shitter](https://f-droid.org/packages/org.nuclearfog.twidda)** was updated from 3.4.3 to 3.4.4
* **[Signal Generator](https://f-droid.org/packages/org.billthefarmer.siggen)** was updated from 1.33 to 1.34
* **[Simple Bitcoin Wallet](https://f-droid.org/packages/com.btcontract.wallet)** was updated from 2.5.4 to 2.5.7
* **[Simple Keyboard](https://f-droid.org/packages/com.simplemobiletools.keyboard)** was updated from 5.4.8 to 5.4.9
* **[Simple Music Player](https://f-droid.org/packages/com.simplemobiletools.musicplayer)** was updated from 5.18.1 to 5.18.3
* **[Sithakuru](https://f-droid.org/packages/kasun.sinhala.keyboard)** was updated from 1.0.9 to 1.1.0
* **[Spotube](https://f-droid.org/packages/oss.krtirtho.spotube)** was updated from 3.1.2 to 3.2.0
* **[Squawker](https://f-droid.org/packages/org.ca.squawker)** was updated from 3.4.4 to 3.5.0
* **[Standard Notes](https://f-droid.org/packages/com.standardnotes)** was updated from 3.167.25 to 3.178.5
* **[Stingle Photos](https://f-droid.org/packages/org.stingle.photos)** was updated from 2.10.2 to 2.11.0
* **[SUD💜KU](https://f-droid.org/packages/com.thesuncat.sudoku)** was updated from 1.1.3 to 2.0.0
* **[Super Retro Mega Wars](https://f-droid.org/packages/com.serwylo.retrowars)** was updated from 0.31.11 to 0.31.12
* **[Table Habit](https://f-droid.org/packages/io.github.friesi23.mhabit)** was updated from 1.9.0 to 1.9.1
* **[Tarnhelm](https://f-droid.org/packages/cn.ac.lz233.tarnhelm)** was updated from 1.5.4 to 1.5.5
* **[Tasks.org: Open-source To-Do Lists & Reminders](https://f-droid.org/packages/org.tasks)** was updated from 13.5.1 to 13.6
* **[Telegram FOSS](https://f-droid.org/packages/org.telegram.messenger)** was updated from 10.0.9 to 10.1.1
* **[Termux:Styling](https://f-droid.org/packages/com.termux.styling)** was updated from 0.30 to 0.31
* **[Tiny Weather Forecast Germany](https://f-droid.org/packages/de.kaffeemitkoffein.tinyweatherforecastgermany)** was updated from 0.61.1 to 0.61.2
* **[TorrServe](https://f-droid.org/packages/ru.yourok.torrserve)** was updated from MatriX.125.2.F-Droid to MatriX.126.1.F-Droid
* **[Transistor - Simple Radio App](https://f-droid.org/packages/org.y20k.transistor)** was updated from 4.1.6 to 4.1.7
* **[TRIfA](https://f-droid.org/packages/com.zoffcc.applications.trifa)** was updated from 1.0.219 to 1.0.220
* **[TU Darmstadt Moodle Wrapper](https://f-droid.org/packages/de.jonasbernard.tudarmstadtmoodlewrapper)** was updated from 1.1 to 1.2
* **[Unciv](https://f-droid.org/packages/com.unciv.app)** was updated from 4.8.12 to 4.8.14
* **[UnicodePad](https://f-droid.org/packages/jp.ddo.hotmist.unicodepad)** was updated from 2.13.1-fdroid to 2.13.3-fdroid
* **[Unpopular Music Player](https://f-droid.org/packages/de.kromke.andreas.unpopmusicplayerfree)** was updated from 2.80.5 to 2.80.6
* **[Unstoppable Wallet](https://f-droid.org/packages/io.horizontalsystems.bankwallet)** was updated from 0.35.1 to 0.36.0
* **[VES - Image and Photo Compare](https://f-droid.org/packages/com.vincentengelsoftware.vesandroidimagecompare)** was updated from 2.2.0 to 2.2.1
* **[Vespucci](https://f-droid.org/packages/de.blau.android)** was updated from 19.2.1.0 to 19.2.3.0
* **[Vinyl Music Player](https://f-droid.org/packages/com.poupa.vinylmusicplayer)** was updated from 1.5.3 to 1.5.5
* **[Voyager for Lemmy](https://f-droid.org/packages/app.vger.voyager)** was updated from 1.15.6 to 1.16.0
* **[WallmeWallpaper:Wallpaper app](https://f-droid.org/packages/com.alaory.wallmewallpaper)** was updated from 2.9 to 3.0
* **[WallpaperExport](https://f-droid.org/packages/com.github.cvzi.wallpaperexport)** was updated from 1.0.3 to 1.1.0
* **[WebCall](https://f-droid.org/packages/timur.webcall.callee)** was updated from 1.2.7 to 1.4.11
* **[Website Monitor](https://f-droid.org/packages/com.manimarank.websitemonitor)** was updated from 2.0.0 to 3.0.0
* **[WG Tunnel](https://f-droid.org/packages/com.zaneschepke.wireguardautotunnel)** was updated from 3.1.0 to 3.1.4
* **[Wikipedia](https://f-droid.org/packages/org.wikipedia)** was updated from r/2.7.50454-r-2023-10-10 to r/2.7.50455-r-2023-10-10
* **[WordleSolver](https://f-droid.org/packages/org.billthefarmer.solver)** was updated from 1.07 to 1.08
* **[wX](https://f-droid.org/packages/joshuatee.wx)** was updated from 55835 to 55836
* **[Xtra](https://f-droid.org/packages/com.github.andreyasadchy.xtra)** was updated from 2.25.2 to 2.25.3
* **[Yivi](https://f-droid.org/packages/org.irmacard.cardemu)** was updated from 7.5.0 to 7.5.1
* **[ZipXtract](https://f-droid.org/packages/com.wirelessalien.zipxtract)** was updated from 2.1 to 2.2
* **[拷贝漫画](https://f-droid.org/packages/top.fumiama.copymanga)** was updated from 2.0.beta20 to 2.0.beta21


Thank you for reading this week's TWIF :).
Please subscribe to the RSS feed at https://f-droid.org/news/ on your favourite RSS application to be updated of new TWIFs when they come up.


You are welcome to join the [TWIF forum thread](https://forum.f-droid.org/t/new-twif-submission-thread/23546) if you have any news from around the community, maybe it will be featured next week.;)

