# MagicGApps
## Copyright (C) 2017-2018, VR25 @ xda-developers
### License: GPL v3+



#### 免责声明

- 本软件以 "现状" 来提供，希望它能有用，但不作任何保证。 在安装/更新之前，请务必阅读参考资料。虽然没有猫受到伤害* ，如因使用/滥用而引致任何问题，我概不负责。
- GNU通用公共许可证第3版或更新的副本将随每个版本一起提供。 请在使用，修改和/或共享此作品的任何部分之前阅读它。
- 为了防止欺诈，不要镜像任何与项目相关的链接。

- \* 原文为 "While no cats have been harmed" 如果你有更好的翻译,请通过issue告诉我


#### 描述

- 以systemlessly方式安装常规open_gapps-*.zip (aroma版除外)。
- 禁用该模块后，Google Play服务也会在下次启动时自动禁用，可防止出现不停的gms崩溃警告



#### 必备条件

- 任何open_gapps-*.zip，aroma版 除外
- 第三方recovery
- Magisk



#### 设置步骤

0. 确保在/sdcard 或/external_sd 目录或子目录中的某处存在open_gapps-*.zip (除了aroma版)
1. 可选的 -- 终端中运行 `touch /data/r` 以 
重装 open_gapps-*.zip (或 `touch 
/data/u` 以卸载模块).
2. 可选的 -- 设置一个gapps-config.txt文件 (删除列表作为伪删除列表 - systemless debloat).
3. 在第三方recovery中安装 (i.e., TWRP).



#### 在线支持

- [Git Repository](https://github.com/Magisk-Modules-Repo/MagicGApps)
- [XDA Thread](https://forum.xda-developers.com/apps/magisk/module-systemless-beansgapps-mini-7-1-x-t3611362)
- [webview_packages: fix incorrect signatures]( https://github.com/LineageOS/android_vendor_cm/commit/a3a76f5d1cc233ad8024ffdc74bb3a786e1605c3)



#### 近期变动

**2018.8.12 (201808120)**
- 添加了GMS Manager脚本 - 在启用/禁用MagicGApps时自动启用/禁用Google Play服务;卸载MagicGApps时自行删除
- 更新了模块说明

**2018.8.11 (201808110)**
- 修复了GApps运行时权限问题
- 修复了“未找到make_ext4fs”（运行Android P的设备）
- 让Open GApps安装程序使用real / persist
- 主要优化和外观变化
- 删除了`gp`可执行文件
- 更新文档

**2018.8.8 (201808080)**
- 添加了Face Unlock相机权限和设置向导相机和位置权限到`gp`

**2018.8.6 (201808060)**
- 添加了gp -- perms授予核心GApps可执行文件
- 次要优化
