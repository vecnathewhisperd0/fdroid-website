---
layout: page
title: Whitelabel Builds

---

F-Droid can be rebranded and embedded in Android ROMs, building upon
F-Droid as the "white-label" version. This is a basic introduction for
how to do that. For this,
["_gradle_ flavors"](https://developer.android.com/studio/build/build-variants.html)
are used for building rebranded, configured versions of F-Droid.

Starting in *app/build.gradle*, add this:

```
android {
    productFlavors {
       mycompany {
           applicationId "com.mycompany.appstore"
       }
    }
}
```

Then *gradle* will automatically look at whole set of folders for custom
versions of files:

- Java sources: _app/src/mycompany/java_
- Manifest file: _app/src/mycompany/AndroidManifest.xml_
- Android resources: _app/src/mycompany/res_
- Assets: _app/src/mycompany/assets_

There cannot be duplicate Java classes, but any extensions can be
managed there. For anything in _res/_, i.e. _strings.xml_ or drawable
resources, the files in _app/src/mycompany/res_ will take precedence
over the default F-Droid ones. For example, override the app icon by
providing _app/src/mycompany/res/drawable/ic\_launcher.xml_.

To specify a custom set of app repositories, provide
_app/src/mycompany/res/values/default\_repos.xml_. The format of that
file is a String array, with sets of 8 elements per repo. For example,
here's the Guardian Project repo config enabled by default with push
request always accepted by the client:

```xml
 <!-- name -->
 <item>Guardian Project</item>
 <!-- address -->
 <item>https://guardianproject.info/fdroid/repo</item>
 <!-- description -->
 <item>
   The official app repository of The Guardian
   Project. Applications in this repository are official
   binaries build by the original application developers and
   signed by the same key as the APKs that are released in the
   Google Play store.
 </item>
 <!-- version -->
 <item>13</item>
 <!-- enabled -->
 <item>1</item>
 <!-- priority -->
 <item>10</item>
 <!-- push requests: ignore, prompt, always -->
 <item>always</item>
 <!-- pubkey -->
 <item>
308205d8308203c0020900a397b4da7ecda034300d06092a864886f70d010105050030d...[snip]
</item>
```

### Customizations

When using gradle build flavors, it is very easy to customize any of
the XML files. So this is the recommended way to start with
customizing your build of F-Droid. Any XML file in _app/src/main/res_
can be overridden by placing an XML with the same name in
_app/src/mycompany/res_. Here are some examples


#### Removing ActionBar/Menu Items

To hide things like "Swap Apps" or "Repositories", override
_app/src/main/res/menu/main.xml_ by copying it into
_app/src/mycompany/res/menu/main.xml_, and removing and/or customizing
the items there.


#### Preferences

For a custom build that enables Automatic Updates by default, override
_app/src/main/res/xml/preferences.xml_. You can customize the
preferences and their default values in
_app/src/mycompany/res/xml/preferences.xml_. The fully automatic
update requires system/root access. With regular access, the updates
will only automatically download. The user still needs to click
install on each one.
