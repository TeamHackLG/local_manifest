Manifest for Android MarshMallow / LineageOS 13.0
====================================
Project M4|L5 / Project U0|L7 / Project V1|L1II / Project Vee3|L3II

---

To initialize LineageOS 13.0 Repo:

    repo init -u https://github.com/LineageOS/android.git -b cm-13.0 -g all,-notdefault,-darwin

---

To initialize Manifest for all devices:

    curl --create-dirs -L -o .repo/local_manifests/roomservice.xml -O -L https://raw.github.com/TeamHackLG/local_manifest/cm-13.0/roomservice.xml

---

Sync the repo:

    repo sync -c --force-sync

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

    brunch v1

---

To build for L3II:

    brunch vee3
