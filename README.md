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

21.input模拟电源键
adb shell input keyevent 26

22.input模拟菜单键
adb shell input keyevent 82

23.input模拟HOME键
adb shell input keyevent 3

24.input模拟返回键
adb shell input keyevent 4

25.点亮屏幕
adb shell input keyevent 224

26.熄灭屏幕
adb shell input keyevent 223

27.滑动解锁
adb shell input swipe 起始点x坐标 起始点y坐标 结束点x坐标 结束点y坐标

28.输入文本
adb shell input text hello

29.截图
adb shell screencap -p /sdcard/test.png

30.日志过滤
按级别，
adb logcat *:W
adb logcat *:D
