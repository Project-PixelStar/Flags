# Flags And Configs #

To Add Maintainer Name In Settings
- usage: Add in DT 'overlay/packages/apps/Settings/res/values/pixelstar_strings.xml'

```bash
<string name="pixelstar_maintainer">yourname</string>
```

To disable Trasparent/Blured recents in pixel launcher

```bash
TARGET_USES_BLUR_RECENT := false
```

For Face Unlock

```bash
TARGET_FACE_UNLOCK_SUPPORTED := true
```

For Offline Charging animation from pixel (RECOMMENDED)

```bash
USE_PIXEL_CHARGER := true
```

For Live Wallpaper

```bash
TARGET_INCLUDE_LIVE_WALLPAPERS := true
```

To Add Quick Tap

```bash
TARGET_SUPPORTS_QUICK_TAP  := true
```

To Remove Aperture Camera

```bash
PRODUCT_NO_CAMERA := true
```

To use Pixel Carrier Settings

```bash
TARGET_INCLUDE_CARRIER_SETTINGS := true
```

Note for including more telephony components

* `TARGET_INCLUDE_PIXEL_IMS`: Pixel IMS
* `TARGET_INCLUDE_PIXEL_EUICC`: Pixel eUICC
* `TARGET_INCLUDE_CARRIER_SERVICES`: Google Carrier Services

If your device support Now Playing feature by Google

```bash
TARGET_SUPPORTS_NOW_PLAYING := true
```

[IMPORTANT]
If you don't want Google Play System to be updatable
(RECOMMENDED) To use this on low end devices with less memory space

```bash
TARGET_SUPPORTS_PREBUILT_UPDATABLE_APEX := false
```

Camera from Google (Formerly, Camera Go or GCam Go)

```bash
TARGET_INCLUDE_CAMERA_GO := true
```

Enabling Android (Go Edition) device specific features

```bash
TARGET_SUPPORTS_LILY_EXPERIENCE := true
```

Build TurboAdapter with dummy GoogleBatteryService when flag is false (RECOMMENDED)

```bash
TARGET_SUPPORTS_GOOGLE_BATTERY := false
```

You can check more Gapps specific flags [**HERE**](https://gitlab.com/pixelstar_gms/vendor_google_gms)