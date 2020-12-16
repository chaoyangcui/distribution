# HarmonyOS开源发行版（HarmonyOS Open-Source Distribution）

HarmonyOS开源发行版（以下简称发行版）是为开发者提供的按需定制的版本，主要目的如下：
1. **向开发者提供按需定制版本** ：以明确的芯片\开发板\模组\Demo等为颗粒度，联合业界合作伙伴交付按需定制的HarmonyOS开源发行版，提升开发人员基于HarmonyOS开发的体验和效率；
2. **向合作伙伴提供最后一公里精准推送能力** ：打通包括[OpenHarmony社区](https://gitee.com/openharmony)、[HarmonyOS包管理（HPM](https://hpm.harmonyos.com/#/cn/home)）、[DevEco IDE工具](https://devecostudio.rnd.huawei.com/download/embedded-studio#download)等在内的发行版分发管道，帮助合作伙伴优化最后一公里发布渠道，更好的推送发行版到开发者手中。
 
 
Distribution仅用于汇总存放官方、第三方HarmonyOS开源发行版的元数据，作为[HarmonyOS包管理（HPM](https://hpm.harmonyos.com/#/cn/home)）、[DevEco IDE工具](https://devecostudio.rnd.huawei.com/download/embedded-studio#download)等后续环节的元数据源头。我们强烈推荐开发者通过[HarmonyOS包管理（HPM](https://hpm.harmonyos.com/#/cn/home)）、[DevEco IDE工具](https://devecostudio.rnd.huawei.com/download/embedded-studio#download)方便快捷的获取HarmonyOS开源发行版。
  
  
HarmonyOS开源发行版设置为两个认证等级，等级将体现在[Distribution仓](https://gitee.com/openharmony/distribution)、[HarmonyOS包管理（HPM](https://hpm.harmonyos.com/#/cn/home)）、[DevEco IDE工具](https://devecostudio.rnd.huawei.com/download/embedded-studio#download)环境中：
-  **官方（Official）** ，源码被[OpenHarmony社区](https://gitee.com/openharmony)正式接纳的HarmonyOS开源发行版。
-  **第三方（3rd-party）** ，满足以下条件之一的HarmonyOS开源发行版：
   - 二进制被[OpenHarmony社区](https://gitee.com/openharmony)正式接纳；
   - 源码被[OpenHarmony-SIG](https://gitee.com/openharmony-sig)（Special Interest Groups）接纳，但尚未被OpenHarmony社区正式接纳；
   - 源码或二进制在[OpenHarmony-SIG]( https://gitee.com/openharmony-sig )及[OpenHarmony社区](https://gitee.com/openharmony)之外的HarmonyOS开源发行版。
  
  
建议Distribution中存放的每个发行版存储的元数据包括：
- bundle.json：要求能准确生成完整依赖
- LICENSE
- README_CN.md
- README_EN.md
- CHANGELOG.md：用于记录该开源发行版的变更，可拆分为中英文两个文件，命名规则同README。
  
  
发行版命名需考虑方便检索，具体规则如下：
- 以芯片驱动为核心，厂商_芯片族(可选)_芯片型号_认证等级，如hisilicon_Hi3861_Official；
- 以单板（开发板/模组）驱动为核心，厂商_板卡型号(可选)_核心芯片型号_认证等级，如BearPi_hm_nano_Hi3861_3rd-party；
- 以应用为核心的Demo，Demo_板卡型号(可选)_核心芯片型号(可选)_Demo名称_认证等级，如Demo_hisilicon_Hi3518EV300_IPCamera_Official。



