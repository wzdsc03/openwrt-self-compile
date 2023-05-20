# openwrt-self-compile
这是一些自编译的openwrt固件，在rom大小上做出调整。
自编译的固件内核版本与官方有区别，导致安装官方的内核模块（kmod）时会提示kernel版本不匹配。为了使后续opkg安装kmod包不产生kernel版本不匹配问题，各个自编译版本编译了所有内核模块（kmod），若在后续使用中遇到kernel版本不匹配的包，使用这里编译的kmod即可。在安装这里的kmod之前，不要opkg update，否则仍然会提示kernel版本不匹配。


The self-compiled firmware kernel version is different from the official firmware version. As a result, when installing the official kernel module (kmod), a message is displayed indicating that the kernel version does not match. In order to avoid the problem of kernel version mismatch when opkg installs kmod packages later, all kernel modules (kmod) are compiled by each self-compiled version. If packages with incompatible kernel versions are encountered in subsequent use, kmod compiled here can be used. Do not "opkg update" before installing kmod  here, otherwise the kernel version mismatch will still be prompted.
