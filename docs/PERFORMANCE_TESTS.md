# Performance tests

| Version | Packet capture engine  |  Achieved capture speed pps/mbps | Hardware | Software platform| Networks and host  number | Packet generator speed | Tool params | 
|:----:|:--:| :----:|:--:| :----:|:--:| :--:| :--:| : --- :|
| [Git commit](https://github.com/FastVPSEestiOu/fastnetmon/commit/0ab076deda7d8d0dc4739f7cc963dca84f62f9a1) | netmap | 7 607 237 pps 3482 mbps | E5-2407  2.20GHz 4 core, ixgbe driver from FastNetMon 10GE load: 100% of all cores | Debian Jessie | Single /24 255 IP| 10GE wire speed 14Mpps, 10GE | Connection tracking disabled. VT-D and hardware virtualization are disabled in BIOS |
| [Git commit](https://github.com/FastVPSEestiOu/fastnetmon/commit/0ab076deda7d8d0dc4739f7cc963dca84f62f9a1) | netmap | 7 506 629 pps 3423 mbps | E5-2407  2.20GHz 4 core, ixgbe driver from FastNetMon 10GE load: 100% of all cores | Debian Jessie | Single /24 255 IP| 10GE wire speed 14Mpps, 10GE | Connection tracking disabled. VT-D and hardware virtualization are enabled in BIOS |
| [Git commit](https://github.com/FastVPSEestiOu/fastnetmon/commit/0ab076deda7d8d0dc4739f7cc963dca84f62f9a1) | PF_RING ZC [git version](https://github.com/ntop/PF_RING/commit/b67a6f46a06e68f2bb6cc53e9d452cc2cbe5f18f) | 5 827 337 pps 2667 mbps | E5-2407  2.20GHz 4 core, ixgbe ZC driver from PF_RING 10GE load: 100% of all cores | Debian Jessie | Single /24 255 IP| 10GE wire speed 14Mpps, 10GE | Connection tracking disabled. VT-D and hardware virtualization are enabled in BIOS |

