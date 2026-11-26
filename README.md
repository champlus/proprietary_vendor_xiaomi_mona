# Proprietary Vendor Blobs for Xiaomi Civi 1 (`mona`)

Extracted from official **Xiaomi HyperOS 1.0 China Stable `OS1.0.2.0.TKVCNXM` (`V816.0.2.0.TKVCNXM`)** for [champlus/android_device_xiaomi_mona](https://github.com/champlus/android_device_xiaomi_mona) targeting **crDroid 13 / Android 17 (`17.0`)**.

## Highlights
- Includes all `mona`-specific camera, audio (`ForteMedia` ACDB + `capi_v2_dap_cpdp.so` + `hrtf5c.bin` for ADSP media playback), AW882xx Smart PA, AW8622x haptics, Goodix UDFPS, Synaptics S3908P firmware, thermal, NFC, and sensor blobs (with all ELF/XML fixups from `extract-files.py` already applied).
- **No Git LFS required**: Stock `radio/*.img` bootloader/modem firmware partitions (e.g. 209 MiB `modem.img`) are intentionally omitted so every file stays under GitHub's 100 MiB limit.
- **Prerequisite before flashing**: Ensure your device is already on HyperOS `OS1.0.2.0.TKVCNXM` firmware (or re-run `extract-files.py --only-target --allow-prohibited-files <stock_dump>` locally to bundle the 17 firmware images into the OTA zip).
