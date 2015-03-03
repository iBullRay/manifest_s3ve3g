CyanogenMod 11.0 for Samsung Galaxy S3 Neo || Duos
==================================================

Getting Started
---------------

To get started with Android/CyanogenMod, you'll need to get
familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

Then to sync and build:

    repo init -u git://github.com/CyanogenMod/android.git -b cm-11.0
    curl --create-dirs -L -o .repo/local_manifests/manifest_s3ve3g.xml -O -L https://raw.githubusercontent.com/iBullRay/manifest_s3ve3g/cm-11.0/manifest_s3ve3g.xml
    repo sync
    sh vendor/cm/get-prebuilts
    lunch cm_s3ve3g-userdebug
    mka bacon