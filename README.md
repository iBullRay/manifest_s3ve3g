LineageOS 7.1.2 for Samsung Galaxy S3 Neo
=========================================

Getting Started
---------------

To get started with Android, you'll need to get
familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

Then to sync and build:

    repo init -u git://github.com/LineageOS/android.git -b cm-14.1
    curl --create-dirs -L -o .repo/local_manifests/manifest.xml -O -L https://raw.githubusercontent.com/iBullRay/manifest_s3ve3gxx/cm-14.1/manifest.xml
    repo sync -j*(where * - number of streams per cores,e.g quad core - -j4)
    source build/envsetup.sh
    lunch lineageos_s3ve3gxx-userdebug
    mka bacon
    If you want to build with TWRP, use this: WITH_TWRP=true mka recoveryimage
