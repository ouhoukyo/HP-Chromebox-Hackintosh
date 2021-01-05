# HP Chromebox Hackintosh

基于 OpenCore 0.6.4，仅在 i7-4600u 平台上测试了 mac 10.15.7 Catalina，理论上所有的 Haswell 架构都可以使用，请自行尝试。

## 使用注意

### 有线网络

-   请自行添加`/EFI/OC/Kexts/RealtekRTL8111.kext/Contents/Info.plist`下的`fallbackMAC`地址，例如：`01:23:45:67:89:AB`，建议**不要使用这个例子**，可以自己搜索 mac 地址随机生成。
-   如果显示`以太网电缆已拔出`，请点击`高级-硬件`将配置改为`手动`，将速度改为`100baseTX`。

### 无线网络

-   intel 无线网卡请编辑`/EFI/OC/Kexts/itlwm.kext/Contents/Info.plist`下的 WiFiConfig，设置 ssid(WiFi名，英文) 与 password(Wifi密码)。
-   

## 其他

- 如果你在尝试使用OpenCore安装黑苹果，可以看一下[cattyhouse的oc指导教程](https://github.com/cattyhouse/oc-guide)，我是按照[这个教程](https://github.com/cattyhouse/oc-guide/blob/master/oc-dmg-install.md)来安装的，身边有1G的u盘和WiFi就可以安装，告别百度云下载镜像的龟速。
- 我也是小白，参考了大佬的配置花了一天时间才搞定，如果安装过程有问题，请善用搜索引擎，有耐心，多尝试。
