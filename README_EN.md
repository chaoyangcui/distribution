OpenHarmony Distribution
OpenHarmony Distribution(Hereinafter referred to as Distribution)is a customized version for developers，The main purpose is as follows:

Provide developers with on-demand customized versions: with clear chips/development boards/modules/Demos as granularity, and industry partners to deliver on-demand customized OpenHarmony releases to improve the developer’s experience and efficiency based on OpenHarmony development;
Provide partners with accurate last-mile push capabilities: open up distribution channels including OpenHarmony community, HarmonyOS package management (HPM), DevEco IDE tools, etc., to help partners optimize the last-mile release channel and better push release Version into the hands of the developer.
Distribution is only used to aggregate and store the metadata of official and third-party OpenHarmony releases, as the source of metadata for subsequent links such as HarmonyOS Package Management (HPM) and DevEco IDE tools. We strongly recommend that developers use the HarmonyOS Package Management (HPM) and DevEco IDE tools to quickly and easily obtain the OpenHarmony release. 


OpenHarmony Distribution Set to two certification levels ,The level will be reflected in the Distribution repo, HarmonyOS package management (HPM), DevEco IDE tool environment: 

Official ,Source Code Officially Accepted By OpenHarmony Community's OpenHarmony Distribution
Partner , OpenHarmony releases that meet one of the following conditions, these releases are released and maintained by partners: 
Binary is officially accepted by the OpenHarmony community; 
The source code is accepted by OpenHarmony-SIG (Special Interest Groups), but has not been officially accepted by the OpenHarmony community; 
The source code or binary is in the OpenHarmony-SIG and OpenHarmony distributions outside the OpenHarmony community. 
It is recommended that these metadata to be stored in each release of the Distribution: 

bundle.json：Requires accurate generation of complete dependencies 
LICENSE
README_CN.md
README_EN.md
CHANGELOG.md：It is used to record the changes of the open source release. It can be divided into two files in Chinese and English. The naming rules are the same as README.
The naming of the release should be considered for easy retrieval. The specific rules are as follows: 

Use chip drivers as the naming scheme, manufacturer_chip family (optional)_chip model_certification level, for example hisilicon_Hi3861_Official; 
Take the single board (development board/module) driver as the scheme, manufacturer_board model (optional)_core chip model_certification level, for example BearPi_hm_nano_Hi3861_3rd-party; 
Demo with application as the naming scheme, Demo_board model (optional)_core chip model (optional)_Demo name_certification level, such as Demo_hisilicon_Hi3518EV300_IPCamera_Official. 