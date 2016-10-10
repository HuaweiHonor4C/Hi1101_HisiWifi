# Hi1101 Android HAL

This consists of two parts, a userspace part and a kernel part.

## Kernel

Every file here except the two folders must be placed inside of: `drivers/huawei_platform/connectivity/hisi/hisiwifi`
if you are not using EMUI, because if you don't, the sysfs interface won't be created.

## Userspace

The files inside 'wifi_hal" must be placed inside of: `frameworks/opt/net/wifi/service/lib` (the path might change)
and the files inside 'wifi' must be placed inside of: `hardware/libhardware_legacy/wifi`.

There might be more changes required, like using stock `libwpa_client_hisi.so` or `wpa_supplicant` but it should be pretty easy to implement.
