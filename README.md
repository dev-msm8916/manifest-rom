# Zenx based on Android 10

<p align="center">
<img src="https://github.com/ZenX-OS/XDA/blob/master/Images/ZenX-OS_logo.png" >
</p>

Sync sources:

    $ repo init -u https://github.com/ZenX-OS/android_manifest.git -b ten
	or shallow clone if you don't have much bandwith
    $ repo init -u https://github.com/ZenX-OS/android_manifest.git -b ten  --depth=1
    $ mkdir -p .repo/local_manifests
    $ wget https://raw.githubusercontent.com/MocaRafee/manifest-rom/zenxQ/zenx.xml -O .repo/local_manifests/roomservice.xml
    $ repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

Building for Xiaomi Redmi Note 3 (kenzo/kate)
---------------

To build:

    $ export LC_ALL=C
    $ . build/envsetup.sh
    $ lunch zenx_kenzo-userdebug
    $ brunch zenx_kenzo-userdebug
