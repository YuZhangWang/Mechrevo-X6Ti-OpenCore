# Mechrevo-X6Ti-OpenCore

## 注意

```cpp
#include <iostream>
using namespace std;
int main()
{
 /*
  Your warranty is now void.
  You are working on your own device, and I am not responsible for any
  bricked devices.
 */
 return 0;
 }
```

## 配置信息
| Device       | Mechrevo X6Ti                                     | 
| -----------: | :---------------------------------------------- | 
| Chipset | Intel HM170 |
| CPU          | Intel i7-6700HQ  | 
| GPU | Nvidia Geforce GTX 965m & Intel HD Graphics 530                             |
| Memory       | 2 * 8 GB 2133 Mhz DDR4 from Sumsung          | 
| WinSSD      | SAMSUNG MZNLN256HCHP-000L7                           |
| MacSSD       | Phison SM280128GPMC15B-S10C2               |
|    Hard disk    |    TOSHIBA MQ01ABD100 |
| Audio Card      | Realtek ALC269                   | 
| Wireless Network Adapter | Intel                          | 
| Ethernet Network Adapter | Realtek RTL8168 / RTL8111 |
| Display Panel      | LG LP156WF6-SPB1            | 
| Battery | 10.8 V * 4400 mAh = 47.52 Wh |
| Dimensions | 382 * 266 * 32-35 mm |
| Weight | 2.7 KG |
| I/O Ports | 2 * USB 3.0 + 2 * USB 2.0 + 1 * USB 3.1 Type-C ( Don't support TB and Video output) + SD Slot + Audio-in + Audio-out + HDMI + RJ45 |
| Internal Slots | 1 * m.2 2230 M key for Wireless Network Adapter + 2 * m.2 2280 ( SATA / PCIe ) + 2 * RAM Slots + 2.5 Inch SATA ( 9.5 mm ) |

## 文件夹内容说明
- [BigSur](https://github.com/YuZhangWang/Mechrevo-X6Ti-OpenCore/tree/master/BigSur/EFI)为安装BigSur所需引导OC
- [Catalina](https://github.com/YuZhangWang/Mechrevo-X6Ti-OpenCore/tree/master/Catalina/EFI)为安装Catalina所需引导OC
- [Resources](https://github.com/YuZhangWang/Mechrevo-X6Ti-OpenCore/tree/master/Resources)为OC主题,文件由莫语大佬制作上传在ta的[博客](https://www.cmbs-soft.com/oc-theme-richu/)里
- [one-key-hidpi-master](https://github.com/YuZhangWang/Mechrevo-X6Ti-OpenCore/tree/master/one-key-hidpi-master)为开启hidpi所需文件
- [HeliPort.dmg](https://github.com/YuZhangWang/Mechrevo-X6Ti-OpenCore/blob/master/HeliPort.dmg)为英特尔网卡开启网络所需文件

## 安装Catania步骤
1. 使用Catalina的引导安装Catalina10.15.7  
2. 进系统之后,安装HeliPort,wifi就可以连接了
 
## 安装BigSur步骤  
1. 这个机器要先装Catalina，然后OTA更新为BigSur  
2. 先用Catalina的引导安装Catalina10.15.7  
3. 进系统之后要用HeliPort进行wifi连接  
4. 因为SIP关闭，需要在OC界面空格，按reset nvram，然后重启进mac，检测更新就行  
5. OTA更新成BigSur之后，引导文件换成BigSur的即可  
6. [hidpi开启教程](https://blog.csdn.net/qq_37417018/article/details/113701115)(所需文件已经放在文件夹中)

## 后续
### 成功的部分
- Catalina三卡驱动成功,亮度调节成功,电池读取成功,鼠标运行成功,键盘运行成功,小键盘运行成功
- BigSur三卡驱动成功,亮度调节成功,电池读取成功,鼠标运行成功,键盘运行成功


### 不成功的部分
- SD卡槽读取失败
- 蓝牙不能用
- 雷电接口不能用
- 打印机识别不了


### 还需优化
- Catalina的USB读取速度慢
- BigSur连着副屏启动,会导致主屏黑掉
- BigSur开机连着副屏一段时间之后会导致主屏和副屏一块花屏
- 由于用的是英特尔的网卡,导致虚拟机内没有网络,后期可以换一张博通的网卡
