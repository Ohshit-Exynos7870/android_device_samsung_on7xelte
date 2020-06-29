# TWRP for the Samsung Galaxy J7 Prime

### How to build ###

```bash
# Create dirs
$ mkdir twrp ; cd twrp

# Init repo
$ repo init --depth=1 -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-9.0

# Clone my local repo
$ git clone https://gitlab.com/Universal7870/manifest/android_manifest_samsung_on7xelte.git -b twrp .repo/local_manifests

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ mv device/samsung/on7xelte/build_twrp.sh .
$ . build_twrp.sh on7xelte
```