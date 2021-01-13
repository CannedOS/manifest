 Getting Started:
 ==============

To get started with manifest/CannedOS, you'll need to get familiar with [Repo](https://source.android.com/source/using-repo.html) and Version Control with [Git](https://source.android.com/source/version-control.html).

To initialize your local repository, use a command like this:

```bash
repo init -u https://github.com/CannedOS/manifest.git -b ravioli

```
You can alternatively use this command to save some space and time :

```bash
repo init --depth=1 -u https://github.com/CannedOS/manifest.git -b ravioli

```

Then to sync up:

```
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
You can just use `repo sync` or above command, but this will save you from lot of terminal spam, data and time.
```bash
repo sync -c -q --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune -j$(nproc --all)
```
---------------------------------------------------------------------------------------
 Compilation of CannedOS:
 ==================

From root directory of project, perform following commands in terminal

```bash
$ . build/envsetup.sh
$ lunch canned_<device_codename>-buildtype
$ mka canned
```
---------------------------------------------------------------------------------------
 Team CannedOS
 ===============

 * [**CannedShroud(Vyom Desai)**](https://t.me/CannedShroudted) - Founder & Lead Developer
 
---------------------------------------------------------------------------------------
 Credits:
 =======

 * [**AOSP**](https://github.com/AOSP)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**ManyMore from where cherry-picked from**](https://github.com)

---------------------------------------------------------------------------------------
'+