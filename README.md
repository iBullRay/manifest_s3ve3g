AOSP 7.1.2 for Samsung Galaxy S3 Neo
====================================

Getting Started
---------------

To get started with Android, you'll need to get
familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

Then to sync and build:

    repo init -u https://android.googlesource.com/platform/manifest -b android-7.1.2_r36
    repo sync -j*(where * - number of streams per cores,e.g quad core - -j4)
    curl --create-dirs -L -o .repo/local_manifests/manifest.xml -O -L https://raw.githubusercontent.com/iBullRay/manifest_s3ve3gxx/aosp-7/manifest.xml
    repo sync -j*(where * - number of streams per cores,e.g quad core - -j4)
    source build/envsetup.sh
    lunch aosp_s3ve3gxx-userdebug
    make -j4 otapackage
