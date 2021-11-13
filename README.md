[poweroffdevice 设备关机功能](luci-app-poweroffdevice)
==========================================
修改自sirpdboy的luci-app-poweroffdevice
源码来源：https://github.com/sirpdboy/luci-app-poweroffdevice

poweroffdevice是一款基于OPNEWRT编译的关机源码插件。
-

大佬的源码一直无法编译，翻译文件里面也有问题，我又不想去改luci的文件。。。  
此版本可以在lede的源码上编译，并添加了关机前有未保存内容的警告。


## 使用说明：

 ```Brach
    # 下载源码
    
    git clone https://github.com/lzq98/luci-app-poweroffdevice
    
    make menuconfig
 ``` 
 ```Brach
    # 配置菜单
    make menuconfig
	# 找到 LuCI -> Applications, 选择 luci-app-poweroffdevice, 保存后退出。
 ``` 
 ```Brach 
    # 编译固件
    make package/luci-app-poweroffdevice/{clean,compile} V=s
 ```
