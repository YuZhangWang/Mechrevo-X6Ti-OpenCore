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
| Memory       | 8 GB 2133 Mhz DDR4 from Sumsung          | 
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

## 安装Catania步骤

## 安装BigSur步骤  
1. 这个机器要先装Catalina，然后OTA上去，之后更新就没问题了   
2. 先用Catalina的引导安装Catalina10.15.7  
3. 进系统之后要用HeliPort进行wifi连接  
4. 因为SIP关闭，需要在OC界面空格，按reset nvram，然后重启进mac，检测更新就行  
5. OTA更新成BigSur之后，引导文件换成BigSur的即可  
6. [hidpi开启教程](https://blog.csdn.net/qq_37417018/article/details/113701115)

## 
