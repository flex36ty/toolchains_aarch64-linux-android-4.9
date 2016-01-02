# toolchains_aarch64-linux-android-4.9

to build kernel 
set .bash.rc path "export PATH=~/android/toolchains/aarch64-linux-android-4.9/bin:$PATH"
copy toolchain to same location

<br>export ARCH=arm64
export SUBARCH=arm64
export CROSS_COMPILE=aarch64-linux-android-
make angler_defconfig
