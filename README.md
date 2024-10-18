# Patches for Peridot

### UDFPS

```bash
cd frameworks/base
wget https://raw.githubusercontent.com/poco-f6-peridot/patch-peridot/peridot-15/UDFPS/0001-DNM-SystemUI-Add-xiaomi-fingerprintextension.patch && \
patch -p1 <0001-DNM-SystemUI-Add-xiaomi-fingerprintextension.patch
cd ../..
```

### Dolby patches

```bash
cd frameworks/av
wget https://raw.githubusercontent.com/poco-f6-peridot/patch-peridot/peridot-15/Dolby/0001-libstagefright-omx-Add-support-for-loading-prebuilt-.patch && \
wget https://raw.githubusercontent.com/poco-f6-peridot/patch-peridot/peridot-15/Dolby/0002-Add-AC4Tbl-params-for-dolby-AC4-decoder-1-2.patch && \
wget https://raw.githubusercontent.com/poco-f6-peridot/patch-peridot/peridot-15/Dolby/0003-media-OMXStore-Import-loading-libstagefrightdolby.patch && \
wget https://raw.githubusercontent.com/poco-f6-peridot/patch-peridot/peridot-15/Dolby/0004-OMX-Remove-support-for-prebuilt-ac4-decoder.patch && \
wget https://raw.githubusercontent.com/poco-f6-peridot/patch-peridot/peridot-15/Dolby/0005-media-Add-changes-to-pick-target-specific-media-xml-.patch && \
wget https://raw.githubusercontent.com/poco-f6-peridot/patch-peridot/peridot-15/Dolby/0006-MediaProfiles-Check-before-overriding-media-settings.patch && \
patch -p1 <0001-libstagefright-omx-Add-support-for-loading-prebuilt-.patch && \
patch -p1 <0002-Add-AC4Tbl-params-for-dolby-AC4-decoder-1-2.patch && \
patch -p1 <0003-media-OMXStore-Import-loading-libstagefrightdolby.patch && \
patch -p1 <0004-OMX-Remove-support-for-prebuilt-ac4-decoder.patch && \
patch -p1 <0005-media-Add-changes-to-pick-target-specific-media-xml-.patch && \
patch -p1 <0006-MediaProfiles-Check-before-overriding-media-settings.patch
cd ../..
```

```bash
cd frameworks/native
wget https://raw.githubusercontent.com/poco-f6-peridot/patch-peridot/peridot-15/Dolby/0001-Add-AC4Tbl-params-for-dolby-AC4-decoder-2-2.patch && \
patch -p1 <0001-Add-AC4Tbl-params-for-dolby-AC4-decoder-2-2.patch
cd ../..
```

### MiuiCamera patches

```bash
cd frameworks/base
wget https://raw.githubusercontent.com/poco-f6-peridot/patch-peridot/peridot-15/Memecamera/0001-Expose-aux-camera-if-packagename-is-null.patch && \
wget https://raw.githubusercontent.com/poco-f6-peridot/patch-peridot/peridot-15/Memecamera/0002-Add-backwards-compatible-CaptureResultExtras-constructor.patch && \
wget https://raw.githubusercontent.com/poco-f6-peridot/patch-peridot/peridot-15/Memecamera/0003-Dont-crash-when-checking-input-configuration-failed.patch && \
wget https://raw.githubusercontent.com/poco-f6-peridot/patch-peridot/peridot-15/Memecamera/0004-Update-HIDL-overrideFormat-from-HAL.patch && \
patch -p1 <0001-Expose-aux-camera-if-packagename-is-null.patch && \
patch -p1 <0002-Add-backwards-compatible-CaptureResultExtras-constructor.patch && \
patch -p1 <0003-Dont-crash-when-checking-input-configuration-failed.patch && \
patch -p1 <0004-Update-HIDL-overrideFormat-from-HAL.patch
cd ../..
```
