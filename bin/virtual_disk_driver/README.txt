这是基于Storport磁盘驱动框架的虚拟磁盘驱动，
支持WIN7以上的系统（WIN7,WIN8,WIN10)，此驱动不再支持WINXP。
安装成功之后，windows系统会把生成的虚拟磁盘当成真正的磁盘。
能在磁盘管理器中进行管理，能在设备管理器中查询到。

安装办法：
打开 设备管理器，操作-> 添加过时硬件，一路“下一步”，直到选择从磁盘安装，
进入对应的驱动目录下，选择 xfs_disk.inf，
会出现 “Fanxiushu xFsRedir Virtual SCSI Adapter”，然后安装。
安装成功之后，会在设备管理器中的“存储控制器中”看到“Fanxiushu xFsRedir Virtual SCSI Adapter”的设备。

驱动签名签名情况：
驱动没做任何签名，如果想要安装成功，需要你自己签名，
或者 WIN7重启按F8，WIN10 按住 Shift + 重启， 进入”配置启动“，选择禁用驱动强制签名。
或者通过bcdedit命令设置永久禁用签名，请留意此种做法带来的内核安全隐患。
如果是最新的WIN10电脑，请确保BIOS中的Secure Boot禁用。

使用办法：
驱动安装成功之后，可以直接打开xFsRedir.exe程序，可以在”添加虚拟磁盘驱动“中
选择使用哪种方式创建虚拟磁盘。
如果选择“主驱动内置的虚拟磁盘”，则任然使用原先方式创建虚拟磁盘。
如果选择“扩展虚拟磁盘驱动”，则使用本驱动创建虚拟磁盘。

