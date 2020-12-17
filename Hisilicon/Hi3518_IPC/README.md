# ip_camera_hi3518ev300

## 开发版介绍

Hi3518EV300作为新一代智慧视觉处理SOC，集成新一代ISP(Image Signal Processor)以及业界最新的H.265视频压缩编码器，同时采用先进低功耗工艺和低功耗架构设计，使其在低码率、高画质、低功耗等方面引领行业水平。

## 功能特性
| 组件名                                    | 能力介绍                                                     |
| ----------------------------------------- | ------------------------------------------------------------ |
| DFX   (DFX)                               | 提供DFX能力。包括：流水日志、时间打点等。                    |
| 分布式调度子系统（Distributed_scheduler） | 通过主从设备服务代理机制，在操作系统上建立起分布式服务平台，支持主设备启动从设备(IP Camera、运动手表等小内存设备)FA的能力。 |
| 多媒体子系统   （MultiMedia）             | 提供相机、音频、视频、音视频编码能力。                       |
| 安全子系统   （Security）                 | 提供应用验签、加解密、设备安全绑定、权限管理、安全态服务等能力。 |
| 启动恢复子系统（StartUp）                 | 提供子系统启动时，加载关键服务能力                           |
| ACE开发框架子系统   (AppFrameworks)       | 提供JS开发框架能力                                           |
| 内核子系统   (Kernel)                     | 提供进程、调度、内存管理等能力                               |
| 驱动子系统   (Driver)                     | 提供驱动框架，包括驱动加载、驱动服务管理和驱动消息机制。     |

## 如何使用

创建一个新的发行版继承自本发行版

```shell
hpm init -t dist
hpm i @ohos/ip_camera_hi3518ev300
```

执行发行命令

```shell
hpm dist
```

## 示例代码

源码目录applications/sample/camera/app/src内**helloworld.c**

```c++
#include <stdio.h>
#include "los_sample.h"

int main(int argc, char **argv)
{
    printf("\n************************************************\n");
    printf("\n\t\tHello world!\n");
    printf("\n************************************************\n\n");
    LOS_Sample(g_num);
    return 0;
}
```

## 参考资料

- Hi3518快速入门
