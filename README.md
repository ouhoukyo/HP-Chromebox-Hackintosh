# HP Chromebox G1 (ZAKO) Hackintosh

基于 OpenCore 0.8.2，仅在 i7-4600u 平台上测试了 mac 10.15.7 Catalina，理论上所有的 Haswell 架构都可以使用，请自行尝试。

## 使用注意 & 存在的问题

### HD4400核心显卡

-   HDMI音频没有声音请[更新BIOS](https://mrchromebox.tech/#fwscript)，注意更新之后会有一些[问题](#bios)。
-   3840x2160分辨率下刷新率仅支持30Hz。

### Rtl有线网络

-   如果显示`以太网电缆已拔出`，请点击`高级-硬件`将配置改为`手动`，将速度改为`100baseTX`。

### Intel无线网络

**本仓库Intel无线驱动仅适用于 Catalina ， Big Sur 用户请自行修改驱动**

请关注[这个仓库](https://github.com/OpenIntelWireless/itlwm)获取最新更新

-   无法连接隐藏网络
-   无法跑满带宽

### Intel蓝牙

请关注[这个仓库](https://github.com/OpenIntelWireless/IntelBluetoothFirmware)获取最新更新

-   连接不稳定
-   部分蓝牙搜索不到

### BIOS

**更新 Coreboot 4.16 后发现关机会自动重启**，暂无修复方法。

## 其他

-   如果你在尝试使用OpenCore安装黑苹果，可以看一下[cattyhouse的oc指导教程](https://github.com/cattyhouse/oc-guide)，我是按照[这个教程](https://github.com/cattyhouse/oc-guide/blob/master/oc-dmg-install.md)来安装的，身边有1G的u盘和WiFi就可以安装。
-   我也是小白，参考了大佬的配置花了一天时间才搞定，如果安装过程有问题，请善用搜索引擎，有耐心，多尝试。
-   如果这个设备没有出手，我会持续更新本仓库。
