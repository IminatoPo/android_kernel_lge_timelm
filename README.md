=========================
android_kernel_lge_timelm
=========================
LG V60 ThinQ A13 kernel source, LMV600TM_kernel_T, TM0_40a, Downloaded form opensource.lge.com


=====
Build
=====
make 
    ARCH=arm64 
     O=./out 
     REAL_CC=../../../prebuilts/clang/host/linux-x86/clang-r353983c/bin/clang 
     CLANG_TRIPLE=aarch64-linux-gnu- 
     CROSS_COMPILE=../../../prebuilts/gcc/linux-x86/aarch64/aarch64-linux-android-4.9/bin/aarch64-linux-android- 
     DTC_EXT=../../../prebuilts/misc/linux-x86/dtc/dtc 
     vendor/timelm-perf_defconfig

make 
    ARCH=arm64 
     O=./out 
     REAL_CC=../../../prebuilts/clang/host/linux-x86/clang-r353983c/bin/clang 
     CLANG_TRIPLE=aarch64-linux-gnu- 
     CROSS_COMPILE=../../../prebuilts/gcc/linux-x86/aarch64/aarch64-linux-android-4.9/bin/aarch64-linux-android- 
     DTC_EXT=../../../prebuilts/misc/linux-x86/dtc/dtc 
     -j12


============
Linux kernel
============

There are several guides for kernel developers and users. These guides can
be rendered in a number of formats, like HTML and PDF. Please read
Documentation/admin-guide/README.rst first.

In order to build the documentation, use ``make htmldocs`` or
``make pdfdocs``.  The formatted documentation can also be read online at:

    https://www.kernel.org/doc/html/latest/

There are various text files in the Documentation/ subdirectory,
several of them using the Restructured Text markup notation.
See Documentation/00-INDEX for a list of what is contained in each file.

Please read the Documentation/process/changes.rst file, as it contains the
requirements for building and running the kernel, and information about
the problems which may result by upgrading your kernel.
