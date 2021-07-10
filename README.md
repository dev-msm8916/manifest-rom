Sync sources:

    $ repo init -u git://github.com/Los-FE/manifest.git -b lineage-18.1
    $ mkdir -p .repo/local_manifests
    $ wget https://raw.githubusercontent.com/dev-msm8916/manifest-rom/11/11.xml -O .repo/local_manifests/roomservice.xml
    $ repo sync

Building for Xiaomi Redmi 3
---------------

To build:

    $ export LC_ALL=C
    $ . build/envsetup.sh
    $ lunch lineage_ido-userdebug
    $ brunch lineaga_ido-userdebug
