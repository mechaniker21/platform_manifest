[Android Open Kang Project](http://aokp.co)
====================================

![Kanged Unicorn](http://aokp.co/images/cms-images/106.png)

Download the Source
===================

Please read the [AOSP building instructions](http://source.android.com/source/index.html) before proceeding.

Initializing Repository
-----------------------

Initiate core trees without any device/kernel/vendor:

    $ repo init -u https://github.com/Emotroid-Rom/platform_manifest.git -b mm

Sync the repository:

    $ repo sync -c -f -j4 --force-sync --no-clone-bundle

***

Building
--------

After the sync is finished, please read the [instructions from the Android site](http://s.android.com/source/building.html) on how to build.

    . build/envsetup.sh
    lunch trltexx

You can also build (and see how long it took) for specific devices (eg. trltexx) like this:

    . build/envsetup.sh
    lunch aokp_trltexx-userdebug
    mka rainbowfarts

Remember to `make clobber && make clean` every now and then!
