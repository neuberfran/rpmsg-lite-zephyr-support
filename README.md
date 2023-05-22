cd /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite

sudo rm -rf build/

west build -p auto -b pico_pi_m4 remote_echo 

-- west build: generating a build system
CMake Warning at /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/cmake/app/boilerplate.cmake:20 (message):
  Loading of Zephyr boilerplate.cmake directly is deprecated, please use
  'find_package(Zephyr)'
Call Stack (most recent call first):
  CMakeLists.txt:4 (include)

Loading Zephyr default modules (Zephyr base).
-- Application: /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/remote_echo
-- CMake version: 3.24.1
-- Found Python3: /usr/bin/python3.8 (found suitable exact version "3.8.10") found components: Interpreter 
-- Cache files will be written to: /home/neuberfran/.cache/zephyr
-- Zephyr version: 3.3.99 (/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr)
-- Found west (found suitable version "1.0.0", minimum required is "0.7.1")
-- Board: pico_pi_m4
-- ZEPHYR_TOOLCHAIN_VARIANT not set, trying to locate Zephyr SDK
-- Found host-tools: zephyr 0.16.0 (/home/neuberfran/zephyr-sdk-0.16.0)
-- Found toolchain: zephyr 0.16.0 (/home/neuberfran/zephyr-sdk-0.16.0)
-- Found Dtc: /home/neuberfran/zephyr-sdk-0.16.0/sysroots/x86_64-pokysdk-linux/usr/bin/dtc (found suitable version "1.6.0", minimum required is "1.4.6") 
-- Found BOARD.dts: /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/boards/arm/pico_pi_m4/pico_pi_m4.dts
-- Generated zephyr.dts: /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/build/zephyr/zephyr.dts
-- Generated devicetree_generated.h: /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/build/zephyr/include/generated/devicetree_generated.h
-- Including generated dts.cmake file: /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/build/zephyr/dts.cmake
Parsing /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/remote_echo/Kconfig
Loaded configuration '/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/boards/arm/pico_pi_m4/pico_pi_m4_defconfig'
Merged configuration '/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/remote_echo/prj.conf'
Configuration saved to '/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/build/zephyr/.config'
Kconfig header saved to '/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/build/zephyr/include/generated/autoconf.h'
-- Found GnuLd: /home/neuberfran/zephyr-sdk-0.16.0/arm-zephyr-eabi/bin/../lib/gcc/arm-zephyr-eabi/12.2.0/../../../../arm-zephyr-eabi/bin/ld.bfd (found version "2.38") 
-- The C compiler identification is GNU 12.2.0
-- The CXX compiler identification is GNU 12.2.0
-- The ASM compiler identification is GNU
-- Found assembler: /home/neuberfran/zephyr-sdk-0.16.0/arm-zephyr-eabi/bin/arm-zephyr-eabi-gcc
CMake Warning at /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/CMakeLists.txt:861 (message):
  No SOURCES given to Zephyr library: drivers__clock_control

  Excluding target from build.


CMake Warning at /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/CMakeLists.txt:861 (message):
  No SOURCES given to Zephyr library: drivers__ipm

  Excluding target from build.


-- Configuring done
-- Generating done
-- Build files have been written to: /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/build
-- west build: building application
[1/149] Preparing syscall dependency handling

[3/149] Generating include/generated/version.h
-- Zephyr version: 3.3.99 (/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr), build: zephyr-v3.3.0-4123-gd01780fc9403
[13/149] Building C object CMakeFiles/app.dir/home/neuberfran/d..._lite/porting/platform/imx7d_m4/rpmsg_platform_zephyr_ipm.c.obj
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/porting/platform/imx7d_m4/rpmsg_platform_zephyr_ipm.c: In function 'platform_init':
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/porting/platform/imx7d_m4/rpmsg_platform_zephyr_ipm.c:249:16: warning: assignment discards 'const' qualifier from pointer target type [-Wdiscarded-qualifiers]
  249 |     ipm_handle = device_get_binding("MU_B");
      |                ^
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/porting/platform/imx7d_m4/rpmsg_platform_zephyr_ipm.c:256:39: warning: passing argument 2 of 'ipm_register_callback' from incompatible pointer type [-Wincompatible-pointer-types]
  256 |     ipm_register_callback(ipm_handle, platform_ipm_callback, NULL);
      |                                       ^~~~~~~~~~~~~~~~~~~~~
      |                                       |
      |                                       void (*)(void *, uint32_t,  volatile void *) {aka void (*)(void *, unsigned int,  volatile void *)}
In file included from /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/porting/platform/imx7d_m4/rpmsg_platform_zephyr_ipm.c:42:
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/include/zephyr/drivers/ipm.h:166:57: note: expected 'ipm_callback_t' {aka 'void (*)(const struct device *, void *, unsigned int,  volatile void *)'} but argument is of type 'void (*)(void *, uint32_t,  volatile void *)' {aka 'void (*)(void *, unsigned int,  volatile void *)'}
  166 |                                          ipm_callback_t cb, void *user_data)
      |                                          ~~~~~~~~~~~~~~~^~
[15/149] Building C object CMakeFiles/app.dir/home/neuberfran/d...pport/lib/rpmsg_lite/porting/environment/rpmsg_env_zephyr.c.obj
FAILED: CMakeFiles/app.dir/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/porting/environment/rpmsg_env_zephyr.c.obj 
/home/neuberfran/zephyr-sdk-0.16.0/arm-zephyr-eabi/bin/arm-zephyr-eabi-gcc -DKERNEL -D__PROGRAM_START -D__ZEPHYR__=1 -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/drivers -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/remote_echo/../../../../../../zephyr/samples/subsys/ipc/rpmsg_lite -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/remote_echo/../../../../../../lib/include -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/remote_echo/../../../../../../lib/include/platform/imx7d_m4 -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/include -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/build/zephyr/include/generated -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/soc/arm/nxp_imx/mcimx7_m4 -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/modules/hal/cmsis/CMSIS/Core/Include -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/modules/hal/nxp/imx/drivers/. -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/modules/hal/nxp/imx/devices/. -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/modules/hal/nxp/imx/devices/MCIMX7D/. -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/modules/hal_nxp/. -isystem /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/lib/libc/minimal/include -isystem /home/neuberfran/zephyr-sdk-0.16.0/arm-zephyr-eabi/bin/../lib/gcc/arm-zephyr-eabi/12.2.0/include -isystem /home/neuberfran/zephyr-sdk-0.16.0/arm-zephyr-eabi/bin/../lib/gcc/arm-zephyr-eabi/12.2.0/include-fixed -fno-strict-aliasing -Os -imacros /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/build/zephyr/include/generated/autoconf.h -ffreestanding -fno-common -g -gdwarf-4 -fdiagnostics-color=always -mcpu=cortex-m4 -mthumb -mabi=aapcs --sysroot=/home/neuberfran/zephyr-sdk-0.16.0/arm-zephyr-eabi/arm-zephyr-eabi -imacros /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/include/zephyr/toolchain/zephyr_stdint.h -Wall -Wformat -Wformat-security -Wno-format-zero-length -Wno-pointer-sign -Wpointer-arith -Wexpansion-to-defined -Wno-unused-but-set-variable -Werror=implicit-int -fno-pic -fno-pie -fno-asynchronous-unwind-tables -fno-reorder-functions --param=min-pagesize=0 -fno-defer-pop -fmacro-prefix-map=/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/remote_echo=CMAKE_SOURCE_DIR -fmacro-prefix-map=/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr=ZEPHYR_BASE -fmacro-prefix-map=/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite=WEST_TOPDIR -ffunction-sections -fdata-sections -std=c99 -nostdinc -MD -MT CMakeFiles/app.dir/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/porting/environment/rpmsg_env_zephyr.c.obj -MF CMakeFiles/app.dir/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/porting/environment/rpmsg_env_zephyr.c.obj.d -o CMakeFiles/app.dir/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/porting/environment/rpmsg_env_zephyr.c.obj -c /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/porting/environment/rpmsg_env_zephyr.c
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/porting/environment/rpmsg_env_zephyr.c: In function 'env_sleep_msec':
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/porting/environment/rpmsg_env_zephyr.c:413:13: error: incompatible type for argument 1 of 'k_sleep'
  413 |     k_sleep(num_msec);
      |             ^~~~~~~~
      |             |
      |             int
In file included from /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/include/zephyr/kernel.h:5956,
                 from /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/porting/environment/rpmsg_env_zephyr.c:47:
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/build/zephyr/include/generated/syscalls/kernel.h:91:43: note: expected 'k_timeout_t' but argument is of type 'int'
   91 | static inline int32_t k_sleep(k_timeout_t timeout)
      |                               ~~~~~~~~~~~~^~~~~~~
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/porting/environment/rpmsg_env_zephyr.c: In function 'env_put_queue':
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/porting/environment/rpmsg_env_zephyr.c:577:57: error: incompatible type for argument 3 of 'k_msgq_put'
  577 |         if (0 == k_msgq_put((struct k_msgq*)queue, msg, timeout_ms))
      |                                                         ^~~~~~~~~~
      |                                                         |
      |                                                         int
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/build/zephyr/include/generated/syscalls/kernel.h:1147:83: note: expected 'k_timeout_t' but argument is of type 'int'
 1147 | static inline int k_msgq_put(struct k_msgq * msgq, const void * data, k_timeout_t timeout)
      |                                                                       ~~~~~~~~~~~~^~~~~~~
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/porting/environment/rpmsg_env_zephyr.c: In function 'env_get_queue':
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/porting/environment/rpmsg_env_zephyr.c:601:57: error: incompatible type for argument 3 of 'k_msgq_get'
  601 |         if (0 == k_msgq_get((struct k_msgq*)queue, msg, timeout_ms))
      |                                                         ^~~~~~~~~~
      |                                                         |
      |                                                         int
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/build/zephyr/include/generated/syscalls/kernel.h:1165:77: note: expected 'k_timeout_t' but argument is of type 'int'
 1165 | static inline int k_msgq_get(struct k_msgq * msgq, void * data, k_timeout_t timeout)
      |                                                                 ~~~~~~~~~~~~^~~~~~~
[17/149] Building C object CMakeFiles/app.dir/src/main_remote_echo.c.obj
FAILED: CMakeFiles/app.dir/src/main_remote_echo.c.obj 
/home/neuberfran/zephyr-sdk-0.16.0/arm-zephyr-eabi/bin/arm-zephyr-eabi-gcc -DKERNEL -D__PROGRAM_START -D__ZEPHYR__=1 -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/drivers -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/remote_echo/../../../../../../zephyr/samples/subsys/ipc/rpmsg_lite -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/remote_echo/../../../../../../lib/include -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/remote_echo/../../../../../../lib/include/platform/imx7d_m4 -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/include -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/build/zephyr/include/generated -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/soc/arm/nxp_imx/mcimx7_m4 -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/modules/hal/cmsis/CMSIS/Core/Include -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/modules/hal/nxp/imx/drivers/. -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/modules/hal/nxp/imx/devices/. -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/modules/hal/nxp/imx/devices/MCIMX7D/. -I/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/modules/hal_nxp/. -isystem /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/lib/libc/minimal/include -isystem /home/neuberfran/zephyr-sdk-0.16.0/arm-zephyr-eabi/bin/../lib/gcc/arm-zephyr-eabi/12.2.0/include -isystem /home/neuberfran/zephyr-sdk-0.16.0/arm-zephyr-eabi/bin/../lib/gcc/arm-zephyr-eabi/12.2.0/include-fixed -fno-strict-aliasing -Os -imacros /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/build/zephyr/include/generated/autoconf.h -ffreestanding -fno-common -g -gdwarf-4 -fdiagnostics-color=always -mcpu=cortex-m4 -mthumb -mabi=aapcs --sysroot=/home/neuberfran/zephyr-sdk-0.16.0/arm-zephyr-eabi/arm-zephyr-eabi -imacros /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/include/zephyr/toolchain/zephyr_stdint.h -Wall -Wformat -Wformat-security -Wno-format-zero-length -Wno-pointer-sign -Wpointer-arith -Wexpansion-to-defined -Wno-unused-but-set-variable -Werror=implicit-int -fno-pic -fno-pie -fno-asynchronous-unwind-tables -fno-reorder-functions --param=min-pagesize=0 -fno-defer-pop -fmacro-prefix-map=/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/remote_echo=CMAKE_SOURCE_DIR -fmacro-prefix-map=/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr=ZEPHYR_BASE -fmacro-prefix-map=/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite=WEST_TOPDIR -ffunction-sections -fdata-sections -std=c99 -nostdinc -MD -MT CMakeFiles/app.dir/src/main_remote_echo.c.obj -MF CMakeFiles/app.dir/src/main_remote_echo.c.obj.d -o CMakeFiles/app.dir/src/main_remote_echo.c.obj -c /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/remote_echo/src/main_remote_echo.c
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/remote_echo/src/main_remote_echo.c: In function 'main':
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/remote_echo/src/main_remote_echo.c:104:62: error: incompatible type for argument 10 of 'k_thread_create'
  104 |                         NULL, NULL, NULL, K_PRIO_COOP(7), 0, 0);
      |                                                              ^
      |                                                              |
      |                                                              int
In file included from /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/zephyr/include/zephyr/kernel.h:5956,
                 from /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/remote_echo/src/main_remote_echo.c:6:
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/build/zephyr/include/generated/syscalls/kernel.h:24:211: note: expected 'k_timeout_t' but argument is of type 'int'
   24 | static inline k_tid_t k_thread_create(struct k_thread * new_thread, k_thread_stack_t * stack, size_t stack_size, k_thread_entry_t entry, void * p1, void * p2, void * p3, int prio, uint32_t options, k_timeout_t delay)
      |                                                                                                                                                                                                       ~~~~~~~~~~~~^~~~~
[20/149] Building C object CMakeFiles/app.dir/home/neuberfran/d...ueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/rpmsg_lite.c.obj
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/rpmsg_lite.c: In function 'rpmsg_lite_rx_callback':
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/rpmsg_lite.c:177:49: warning: taking address of packed member of 'struct rpmsg_std_hdr' may result in an unaligned pointer value [-Waddress-of-packed-member]
  177 |             rsvd = (struct rpmsg_hdr_reserved *)&rpmsg_msg->hdr.reserved;
      |                                                 ^~~~~~~~~~~~~~~~~~~~~~~~
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/rpmsg_lite.c: In function 'rpmsg_lite_alloc_tx_buffer':
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/rpmsg_lite.c:716:45: warning: taking address of packed member of 'struct rpmsg_std_hdr' may result in an unaligned pointer value [-Waddress-of-packed-member]
  716 |     reserved = (struct rpmsg_hdr_reserved *)&rpmsg_msg->hdr.reserved;
      |                                             ^~~~~~~~~~~~~~~~~~~~~~~~
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/rpmsg_lite.c: In function 'rpmsg_lite_send_nocopy':
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/rpmsg_lite.c:760:45: warning: taking address of packed member of 'struct rpmsg_std_hdr' may result in an unaligned pointer value [-Waddress-of-packed-member]
  760 |     reserved = (struct rpmsg_hdr_reserved *)&rpmsg_msg->hdr.reserved;
      |                                             ^~~~~~~~~~~~~~~~~~~~~~~~
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/rpmsg_lite.c: In function 'rpmsg_lite_release_rx_buffer':
/home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/lib/rpmsg_lite/rpmsg_lite.c:801:45: warning: taking address of packed member of 'struct rpmsg_std_hdr' may result in an unaligned pointer value [-Waddress-of-packed-member]
  801 |     reserved = (struct rpmsg_hdr_reserved *)&rpmsg_msg->hdr.reserved;
      |                                             ^~~~~~~~~~~~~~~~~~~~~~~~
[24/149] Building C object zephyr/CMakeFiles/zephyr.dir/lib/os/rb.c.obj
ninja: build stopped: subcommand failed.
FATAL ERROR: command exited with status 1: /usr/local/bin/cmake --build /home/neuberfran/diegosueiro/rpmsg-lite-zephyr-support/zephyr/samples/subsys/ipc/rpmsg_lite/build
