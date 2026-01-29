# Opus Flutter Android 16KB Page Size Patch

This folder contains the minimal items needed to make `opus_flutter_android`
build 16KB-page-size compatible `libopus.so` for Android 15+.

## How to use
1. Clone the upstream repo:
   `git clone https://github.com/EPNW/opus_flutter.git`
2. Apply the patch in this folder:
   `git apply opus_flutter_android_16kb.patch`
3. Build or publish your forked `opus_flutter_android`.

## Notes
- The patch pins a modern NDK and adds a linker flag to align at 16KB.
- The plugin uses `ndk-build` via `Android.mk`.
