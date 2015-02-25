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
    brunch s3ve3g

Buildbot
--------

This device is built weekly and periodically as changes are committed to ensure the source trees remain buildable.

You can view the current build status at [Jenkins Build-Server](http://jenkins.build-server.com/job/cm-s3ve3g/)
