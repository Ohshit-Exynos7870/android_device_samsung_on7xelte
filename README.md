# OrangeFox Recovery Project for the Samsung Galaxy J7 Prime

### How to build ###

```bash
# Create dirs
$ mkdir ofox ; cd ofox

# Init repo
$ repo init --depth=1 -u https://gitlab.com/OrangeFox/Manifest.git -b fox_9.0

# Clone my local repo
$ git clone https://gitlab.com/Universal7870/manifest/android_manifest_samsung_on7xelte.git -b orangefox .repo/local_manifests

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ mv device/samsung/on7xelte/build_ofox.sh .
$ . build_ofox.sh on7xelte
```