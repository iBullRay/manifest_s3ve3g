AOSP 7.1.2 for Samsung Galaxy S3 Neo || Duos
============================================

Getting Started
---------------

To get started with Android, you'll need to get
familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

Then to sync and build:

    repo init -u git://github.com/iBullRay/manifest_s3ve3gxx.git -b aosp-7
    repo sync -j*(where * - number of streams per cores,e.g quad core - -j4)
    source build/envsetup.sh
    lunch aosp_s3ve3gxx-userdebug
    make -j4 otapackage
