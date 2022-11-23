# USB_GPIO说明

### 1.硬件说明

ATTINY85部分与USB的连接参考自Digispark<br>

> 资料下载：[Digispark USB Development Board - Digistump](http://digistump.com/products/1)

### 2.程序说明

参考自Github开源项目[I2C-Tiny-USB](https://github.com/harbaum/I2C-Tiny-USB)<br>

### 3.烧录说明

> 参考自[micronucleus](https://github.com/micronucleus/micronucleus)

以下烧录基于Win10系统，且仅适用于烧录好bootloader的ATTINY85，Linux系统下参考[I2C-Tiny-USB](https://github.com/harbaum/I2C-Tiny-USB)<br>

1）下载相关软件包[micronucleus](https://github.com/micronucleus/micronucleus)并解压<br>

2）将开源项目[I2C-Tiny-USB](https://github.com/harbaum/I2C-Tiny-USB)下的main.hex文件复制到firmware\releases目录下<br>

3）将commandline\builds\i686-mingw32目录下的micronucleus.exe复制到firmware\releases目录下<br>

4）打开文件夹中的windows_driver_installer，运行zadig.exe文件安装micronucleus。安装教程见当前文件夹中Readme。<br>

5）打开文件夹中的firmware，接着打开文件夹releases，在该文件夹下打开cmd，执行指令micronucleus --run main.hex<br>

6）待Pleass plug in the device ...提示弹出后将设备接入电脑，等待烧录进度完成即可<br>

### 注：

参考资料：<br>

1）[DigiSpark更新Bootloader_hexesdesu的博客-CSDN博客](https://blog.csdn.net/sxhexin/article/details/87914649)

2）[MicroNucleus bootloader upgrade (iot-experiments.com)](https://www.iot-experiments.com/micronucleus-bootloader-upgrade/)

3）[基于ATTiny85的digispark Arduino最小系统的自制教程（二）_Argon_Ghost的博客-CSDN博客_attiny85arduino](https://blog.csdn.net/Argon_Ghost/article/details/103859931)
