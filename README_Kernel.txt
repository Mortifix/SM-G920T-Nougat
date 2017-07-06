################################################################################

1. How to Build
	- get Toolchain
		From android git server , codesourcery and etc ..
		 - arm-eabi-4.9
		
	- edit Makefile
		edit "CROSS_COMPILE" to right toolchain path(You downloaded).
		  EX)  CROSS_COMPILE= $(android platform directory you download)/android/prebuilts/gcc/linux-x86/aarch64/aarch64-linux-android-4.9/bin/aarch64-linux-android- (common_build_conf.zeroflte)
		  Ex)  CROSS_COMPILE=/usr/local/toolchain/arm-eabi-4.9/bin/arm-eabi-		// check the location of toolchain
  	
        - to Build
          $ make zerofltetmo_02_defconfig
          $ make -j64

2. Output files
	- Kernel : arch/arm/boot/zImage
	- module : drivers/*/*.ko

3. How to Clean	
		$ make clean
################################################################################
