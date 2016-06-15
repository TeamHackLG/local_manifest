Manifest for Android KitKat / CyanogenMod 11.0
====================================
Project M4|L5 / Project U0|L7 / Project V1|L1II / Project Vee3|L3II

---

Automatic Way:

script to download manifests, sync repo  and build:

    curl --create-dirs -L -o build.sh -O -L https://raw.github.com/Caio99BR/android_.repo_local_manifests/cm-11.0/build.sh

To use:

    source build.sh

---

Manual Way:

To initialize CyanogenMod 11.0 Repo:

    repo init -u git://github.com/CyanogenMod/android.git -b cm-11.0 -g all,-notdefault,-darwin

---

To initialize Common Manifest for all devices:

    curl --create-dirs -L -o .repo/local_manifests/common_manifest.xml -O -L https://raw.github.com/Caio99BR/android_.repo_local_manifests/cm-11.0/common_manifest.xml

---

To initialize Manifest for L5:

    curl --create-dirs -L -o .repo/local_manifests/m4_manifest.xml -O -L https://raw.github.com/Caio99BR/android_.repo_local_manifests/cm-11.0/m4_manifest.xml

---

To initialize Manifest for L7:

    curl --create-dirs -L -o .repo/local_manifests/u0_manifest.xml -O -L https://raw.github.com/Caio99BR/android_.repo_local_manifests/cm-11.0/u0_manifest.xml

---

To initialize Manifest for L1II:

    curl --create-dirs -L -o .repo/local_manifests/v1_manifest.xml -O -L https://raw.github.com/Caio99BR/android_.repo_local_manifests/cm-11.0/v1_manifest.xml

---

To initialize Manifest for L3II:

    curl --create-dirs -L -o .repo/local_manifests/vee3_manifest.xml -O -L https://raw.github.com/Caio99BR/android_.repo_local_manifests/cm-11.0/vee3_manifest.xml

---

# Never use 'L5/L7' Manifest with 'L1II/L3II' Manifest

---

Sync the repo:

    repo sync

---

Initialize the environment:

    source build/envsetup.sh

---

To build for L5:

    brunch e610

---

To build for L7:

    brunch p700

---

To build for L1II:

    sh device/lge/v1/patches/apply.sh
    brunch v1

---

To build for L3II:

    sh device/lge/vee3/patches/apply.sh
    brunch vee3
