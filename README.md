# LEDE-OpenWRT-firmware-for-WRT350n-v2

With LuCI, relayd and a patch for [this issue](https://dev.openwrt.org/ticket/13064 "[ath9k][orion][WRT350n v2]: wrong rx_chainmask disables wireless").

Firmware provided as is - only WRT350nv2 sysupgrade image is tested - use it at your own risk.

Specifig changes made for each release are in respective READMEs. 


### BASIC COMPILATION (LEDE r4983 and above):

First, [install build system](https://openwrt.org/docs/guide-developer/build-system/install-buildsystem).
Second, [clone repository](https://openwrt.org/docs/guide-developer/build-system/install-buildsystem#downloading_sources) 
( or [update](https://openwrt.org/docs/guide-developer/build-system/use-buildsystem#updating_sources_with_git) 
if already cloned) and [update and install feeds](https://openwrt.org/docs/guide-developer/build-system/use-buildsystem#updating_feeds).

Then

#### use CONFIG:

Replace `.config` in root of OpenWRT installation with provided `.config` file.

### or

#### use CONFIG seed:

Use provided seed - at `targets/orion/generic/config.{seed or buildinfo}`, and [use it according to compilation manual](https://openwrt.org/docs/guide-developer/build-system/use-buildsystem#configure_using_config_diff_file), whichever method you prefer.


Continue with [download](https://openwrt.org/docs/guide-developer/build-system/use-buildsystem#download_sources_and_multi_core_compile) and, or skip straight to, [building image](https://openwrt.org/docs/guide-developer/build-system/use-buildsystem#building_images).