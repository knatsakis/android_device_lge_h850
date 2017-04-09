## Device tree for LG G5 (International H850)

Add to `.repo/local_manifests/h850.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/lge/h850" name="knatsakis/android_device_lge_h850" remote="github" revision="android-7.0"/>
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_h850-eng
make -j5 recoveryimage
```

Kernel sources are available at: https://github.com/knatsakis/android_kernel_lge_msm8996

