#WM
使用WIFI模块自带MCU开发在工程配置添加ZC_MODULE_DEV宏定义
需要 App\Adapter\ZC\inc\tropicssl\secconfig.h文件TROPICSSL_HAVE_ASM注释掉，否则联盛的编译汇编代码会出错
##1.AC_WM_v1.0.0_20150916
AbleCloud联盛德代码版本入库
##2.AC_WM_v1.0.1_20151009
优化内存空间
##3.AC_WM_v1.0.2_20151223
1.支持简化协议2.2版本
2.解决局域网控制跑死的问题，初步怀疑是由于联盛德串口发送是异步导致。
后面内存释放，真正发送串口数据时，内存已释放。导致跑死
3.添加oneshot按键