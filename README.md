# toolchains_aarch64-linux-android-4.9

to build kernel 
set .bash.rc path "export PATH=~/android/toolchains/aarch64-linux-android-4.9/bin:$PATH"
copy toolchain to same location

open terminal
<br>export ARCH=arm64
<br>export SUBARCH=arm64
<br>export CROSS_COMPILE=aarch64-linux-android-
<br>make angler_defconfig

<br>sudo apt-get install git build-essential abootimg
<br>copy boot img to folder
<br>abootimg -x boot.img
<br>replace zImage-dtb
<br>sed -i '/bootsize =/d' bootimg.cfg
<br>abootimg --create newboot.img -f bootimg.cfg -k zImage-dtb -r initrd.img
