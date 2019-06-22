<p align="center">
<img src="https://github.com/AospExtended/manifest/raw/7.1.1/aex_logo.png" width="320px" height="320px" > 
</p>

AospExtended Oreo
===========
AospExtended is just an extension to AOSP, through which we 
are trying to provide a stock AOSP experience along with some important 
customization features. We have cherry-picked the features from many 
other projects and hence we are very thankful to them.

Credits
-------
* [**JDCTeam**](https://github.com/AOSP-JF-MM)
* [**DirtyUnicorns**](https://github.com/DirtyUnicorns)
* [**TeamSubstratum (Theme Engine)**](https://github.com/Substratum)
* [**LineageOS/Cyanogenmod**](https://github.com/LineageOS)
* [**Nitrogen Project**](https://github.com/nitrogen-project)
* [**ABC ROM**](https://github.com/ezio84)
* [**GZOSP**](https://github.com/GZOSP)
* [**Pure Nexus**](https://github.com/PureNexusProject)
* [**OmniROM**](https://github.com/omnirom/)
* [**AOSPA**](https://github.com/aospa/)
* [**BlissRoms**](https://github.com/BlissRoms)

Contributors for my project
-------
* [**Victor Shilin**](https://github.com/ChronoMonochrome) LOS 16.0 Builder
* [**Dan Santos**](https://github.com/linusdan) My Mentor, who taught me how to make ROMs
* [**Jarl-Penguin**](https://github.com/JarlPenguin) For some contribution in what files should be there and build error fixing
* [**Ciyanogen**](https://github.com/ciyanogen) For finding errors in my manifest

How to Build?
-------------

To initialize a shallow clone, which will save even more space & time, use a command like this:

```bash
  repo init --depth=1 -u git://github.com/AospExtended/manifest.git -b 8.1.x
```

Clone my repo:
----------------

```bash
git clone https://github.com/aex-i9300/platform_manifests.git -b 8.1.x .repo/local_manifests
``` 

Then to sync up:
----------------

```bash
  repo sync -c --force-sync --no-clone-bundle --no-tags
```
Finally to build:
-----------------
From root directory of Project, perform following commands in terminal

```bash
git clone https://github.com/aex-i9300/platform_manifests.git -b 8.1.x
. build/envsetup.sh
bash platform_manifests/fetch.sh
bash platform_manifests/apply.sh
```

Altering the subject line to reflect your information:
```bash
subject='/C=US/ST=California/L=Mountain View/O=Android/OU=Android/CN=Android/emailAddress=android@android.com'
mkdir .android-certs
for x in releasekey platform shared media testkey; do \
    ./development/tools/make_key .android-certs/$x "$subject"; \
done
```

```bash
  . build/envsetup.sh
  lunch aosp_i9300-userdebug
  make -jX aex  | tee log.txt
```

## Report build issues
- You can reach us via [Telegram](https://t.me/aospextendedgroup)

## Maintain Officially
- If you're building **AospExtended** for an unofficial device and would like to make it official, Check out the link below for more information about the requirements for both you and your device.  
- [Click here for more info](https://github.com/AospExtended/Documentation_and_thread-template) (**Read full README**)

### Important Links:

- [Website](http://www.aospextended.com/)
- [Download Center](https://downloads.aospextended.com/)
- [Blog](https://blog.aospextended.com/)
- [Gerrit Code Review](http://gerrit.aospextended.com/)
- [Telegram Channel](https://telegram.me/aospextended/)
- [Documentation & Thread Template](https://github.com/AospExtended/Documentation_and_thread-template/) 
- [Help us translate AospExtended ROM and bring it to the world!](http://translate.aospextended.com/)
- [Theme Resources](https://github.com/AospExtended/AEX-Scripts/) 
- [Extended Devices](https://github.com/AospExtended-devices/)
- [Gallery](https://aospextended.com/gallery)
- [Facebook page!](https://www.facebook.com/aospextended/)
