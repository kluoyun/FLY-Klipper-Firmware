# FLY-Klipper-Firmware
** 为FLY主板自动编译Klipper固件

# 特点
* 每小时构建（Klipper仓库主分支有新的提交时）
* 种类齐全，覆盖所有FLY主板
* 缓存5个历史最新版本固件
* fast加速下载

# 如何开始
1. 查看你的主板型号
2. 进入上方对应主板型号文件夹
3. 点击最后一行的**加速下载**或者**普通下载**
4. 准备一张SD卡，并格式化为FAT32格式
5. 将此处下载的**firmware.bin**复制到SD卡
6. 将SD卡插入FLY主板并通电，等待10秒（后再按一下主板上的重置键，等待10秒）
7. 用usb线将你的树莓派或其他klipper主机与FLY主板连接
8. 进入树莓派或其他klipper主机的ssh
9. 输入**ls /dev/serisl/by-id/\***,返回的就是你的主板的串口地址。（没有输出的话请重复步骤1-9）
10. 将步骤9中得到的串口地址填写到printer.cfg中（[mcu] serial: 串口地址）

# 感谢
[FLYmaker](https://github.com/FLYmaker/)
[Mellow](https://mellow.aliexpress.com/store/1531088)
