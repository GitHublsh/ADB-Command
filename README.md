# ADB-Command
ADB command
1.查看设备
adb devices

2.查看当前Activity
adb shell dumpsys activity activities | grep "Run"

3.获取root权限
adb root

4.安装apk
adb install <apk file>

5.卸载APP
adb uninstall <Package name>

6.清除应用数据与缓存
adb shell pm clear <Package name>
  
7.强制停止应用
adb shell am force-stop <Package name>

8.查看日志
adb log

9.查看序列号
adb get-serialno

10.获取MAC地址
adb shell cat/sys/class/net/wlan0/address

11.查看设备号 
adb shell getprop ro.product.model

12.查看Android系统版本
adb shell getprop ro.build.version.release

13.查看屏幕分辨率
adb shell wm size

14.查看屏幕密度
adb shell wm density

15.显示所有应用
adb shell pm list package

16.调起Activiity
adb shell am start -n com.test.Activity

17.调起service
adb shell am startservice -n com.test.service

18.发起广播
adb shell am broadcast [options] <INTENT>
  
19.拉取手机文件到本地
adb pull <phone path file> <local path>
  
20.复制文件到Android设备
adb push <电脑上的文件路径> <设备里的目录> 

