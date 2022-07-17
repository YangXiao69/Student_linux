# linux学习笔记
## 第一章 linux系统搭建

- u-boot解压 打补丁 编译 最后生成u-boot.bin u-boot就是个单片  
裸机程序，需要用下载器烧写程序。  

- kernal内核的打补丁 编译 。 使用厂家的配置文件 **cp config_ok .config**  

- busybox的生成？

------
网络文件系统 nfs network file system 的挂载上电后手动挂载  
**eg:  mount -t nfs -o nolock 192.168.101.10:/work/nfs_root /mnt**  

**mount -t nfs -o intr,nolock,rsize=1024,wsize=1024 192.168.101.8:/work/nfs_root /mnt**  
设置开发板ip  
**ifconfig eth0 192.168.101.55**
## 第二章 驱动开发

字符设备驱动程序
insmod led.ko  加载驱动
rmmod led 卸载驱动模块
lsmod  查看驱动/模块








