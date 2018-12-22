export PATH=`pwd`/kernel/aarch64-linux-android-4.9/bin:$PATH

make -f `pwd`/kernel/msm-4.4/AndroidKernel.mk INSTALLED_KERNEL_TARGET=`pwd`/out TARGET_KERNEL_ARCH=arm64 TARGET_KERNEL_HEADER_ARCH=arm64 KERNEL_HEADER_DEFCONFIG=sdm660_defconfig TARGET_KERNEL_CROSS_COMPILE_PREFIX=aarch64-linux-android- TARGET_OUT_INTERMEDIATES=out/obj TARGET_KERNEL_APPEND_DTB=true KERNEL_DEFCONFIG=sdm660_defconfig out/obj/kernel/msm-4.4/arch/arm64/boot/Image.gz-dtb TARGET_OUT=`pwd`/out/system
