## honor8
��Ϊ��ҫ8ȫ��ͨˢ�������ROM��ᵼ�µ��ſ�ͨ������������Ϊ����ͨ��ʹ��2G/3G���磬��ҫ8�ԶԵ���2G/3G��CDMA/CDMA2000����֧�ֲ��õ�����һ���оƬ�����ܵ�����Open Kirin�Ĳ�֧�֡���Ҫʹ��4G����ͨ���迪��VoLTE����Open Kirin�ٷ�û����֧��VoLTE��ò����ҫ8Ҳ��֧��VoLTE����

## Unlock
* adb shell getprop
* adb reboot bootloader
* fastboot oem unlock 9297843358022705

## Honor 8  Android 8.0  EMUI 8.0:
* adb reboot bootloader
* fastboot flash recovery_ramdisk twrp-3.2.1-0.img
* fastboot reboot

erecovery  to newest, then downgrade to EMUI 5.0.1 by HiSuite

## Honor 8  Android 7.0  EMUI 5.0.1:
* adb reboot bootloader
* fastboot flash recovery twrp-3.1.1-1-frd.img
* fastboot reboot

XposedInstaller_*.apk from this thread: Must be installed to manage installed modules, the framework won't work without it.

xposed*.zip from https://dl-xda.xposed.info/framework/: Must be flashed with a custom recovery (e.g. TWRP) to install the framework.

SDK21 is Android 5.0 (Lollipop), SDK22 is Android 5.1 (also Lollipop) and SDK23 is Android 6.0 (Marshmallow).

For Nougat, SDK24 is Android 7.0 and SDK25 is Android 7.1.

For Oreo, SDK26 is Android 8.0 and SDK27 is Android 8.1.

I only support the latest Xposed version per Android release!

xposed-uninstaller*.zip from https://dl-xda.xposed.info/framework/: Can be flashed with a custom recovery (e.g. TWRP) to uninstall the framework.


/system/app

/system/priv-app

/cust/all/cn/app

/product/app

/data/hw_init/system/app

/data/hw_init/version/region_comm/china/app

/data/hw_init/version/special_cust/EVA-AL00/all/cn/app


## ����Data������
* adb reboot bootloader
* fastboot flash recovery_ramdisk huawei-honor-8-em8_0-twrp3.2.1-7to-recovery-8.5.18.img
* fastboot reboot
* adb reboot recovery
����Dalvik/ART Cache��Cache��Data����ʽ��Data���߼������Ƴ�Dataǿ�Ƽ���

## ˢ�������ROM�������Ƴ�DATAǿ�Ƽ��ܣ���
* adb reboot bootloader
* fastboot flash system openkirin_rros_beta3.img
* fastboot reboot
