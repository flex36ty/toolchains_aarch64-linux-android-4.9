# toolchains_aarch64-linux-android-4.9

to build kernel 
set .bash.rc path "export PATH=~/android/toolchains/aarch64-linux-android-4.9/bin:$PATH"
copy toolchain to same location

open terminal
<br>export ARCH=arm64
<br>export SUBARCH=arm64
<br>export CROSS_COMPILE=aarch64-linux-android-
<br>make angler_defconfig
