

usermod -a -G video aillusions

sudo lshw

                  *-core
                       description: Motherboard
                       product: Z97-PRO GAMER
                       vendor: ASUSTeK COMPUTER INC.
                       physical id: 0
                       version: Rev X.0x
                       serial: 150850449502340
                       slot: To be filled by O.E.M.
                     *-firmware
                          description: BIOS
                          vendor: American Megatrends Inc.
                          physical id: 0
                          version: 2106
                          date: 05/21/2015
                          size: 64KiB
                          capacity: 8128KiB
                          capabilities: pci apm upgrade shadowing cdboot bootselect socketedrom edd int13floppy1200 int13floppy720 int13floppy2880 int5printscreen int9keyboard int14serial int17printer acpi usb biosbootspecification uefi
                     *-memory
                          description: System Memory
                          physical id: 45
                          slot: System board or motherboard
                          size: 20GiB
                        *-bank:0
                             description: DIMM DDR3 Synchronous 1333 MHz (0.8 ns)
                             product: KHX1600C10D3/8G
                             vendor: Kingston
                             physical id: 0
                             serial: 50219F0A
                             slot: DIMM_A1
                             size: 8GiB
                             width: 64 bits
                             clock: 1333MHz (0.8ns)
                        *-bank:1
                             description: DIMM DDR3 Synchronous 1333 MHz (0.8 ns)
                             product: KHX1600C10D3/8G
                             vendor: Kingston
                             physical id: 1
                             serial: 6E21F852
                             slot: DIMM_A2
                             size: 8GiB
                             width: 64 bits
                             clock: 1333MHz (0.8ns)
                        *-bank:2
                             description: DIMM [empty]
                             product: [Empty]
                             vendor: [Empty]
                             physical id: 2
                             serial: [Empty]
                             slot: DIMM_B1
                        *-bank:3
                             description: DIMM DDR3 Synchronous 1333 MHz (0.8 ns)
                             product: 99U5429-014.A00LF
                             vendor: Kingston
                             physical id: 3
                             serial: 3C2053B3
                             slot: DIMM_B2
                             size: 4GiB
                             width: 64 bits
                             clock: 1333MHz (0.8ns)
                     *-cpu
                          description: CPU
                          product: (Fill By OEM)
                          vendor: Intel Corp.
                          vendor_id: GenuineIntel
                          physical id: 53
                          bus info: cpu@0
                          version: Intel(R) Core(TM) i7-4790K CPU @ 4.00GHz
                          slot: SOCKET 1150
                          size: 800MHz
                          capacity: 4001MHz
                          width: 64 bits
                          clock: 100MHz
                          capabilities: x86-64 fpu fpu_exception wp vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx pdpe1gb rdtscp constant_tsc arch_perfmon pebs bts rep_good xtopology nonstop_tsc aperfmperf pni pclmulqdq dtes64 monitor ds_cpl vmx est tm2 ssse3 fma cx16 xtpr pdcm pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand lahf_lm abm ida arat epb xsaveopt pln pts dtherm tpr_shadow vnmi flexpriority ept vpid fsgsbase bmi1 hle avx2 smep bmi2 erms invpcid rtm cpufreq
                          configuration: cores=4 enabledcores=4 threads=8
                     *-pci
                          description: Host bridge
                          product: 4th Gen Core Processor DRAM Controller
                          vendor: Intel Corporation
                          physical id: 100
                          bus info: pci@0000:00:00.0
                          version: 06
                          width: 32 bits
                          clock: 33MHz
                          configuration: driver=hsw_uncore
                          resources: irq:0
                        *-pci:0
                             description: PCI bridge
                             product: Xeon E3-1200 v3/4th Gen Core Processor PCI Express x16 Controller
                             vendor: Intel Corporation
                             physical id: 1
                             bus info: pci@0000:00:01.0
                             version: 06
                             width: 32 bits
                             clock: 33MHz
                             capabilities: pci pm msi pciexpress normal_decode bus_master cap_list
                             configuration: driver=pcieport
                             resources: irq:31 ioport:e000(size=4096) memory:f7c00000-f7cfffff ioport:e0000000(size=276824064)
                           *-display
                                description: VGA compatible controller
                                product: Bonaire [Radeon R7 200 Series]
                                vendor: Advanced Micro Devices, Inc. [AMD/ATI]
                                physical id: 0
                                bus info: pci@0000:01:00.0
                                version: 00
                                width: 64 bits
                                clock: 33MHz
                                capabilities: pm pciexpress msi vga_controller bus_master cap_list rom
                                configuration: driver=amdgpu latency=0
                                resources: irq:35 memory:e0000000-efffffff(prefetchable) memory:f0000000-f07fffff(prefetchable) ioport:e000(size=256) memory:f7c00000-f7c3ffff memory:f7c40000-f7c5ffff(prefetchable)
                           *-multimedia
                                description: Audio device
                                product: Tobago HDMI Audio [Radeon R7 360 / R9 360 OEM]
                                vendor: Advanced Micro Devices, Inc. [AMD/ATI]
                                physical id: 0.1
                                bus info: pci@0000:01:00.1
                                version: 00
                                width: 64 bits
                                clock: 33MHz
                                capabilities: pm pciexpress msi bus_master cap_list
                                configuration: driver=snd_hda_intel latency=0
                                resources: irq:17 memory:f7c60000-f7c63fff
                        *-display
                             description: Display controller
                             product: Xeon E3-1200 v3/4th Gen Core Processor Integrated Graphics Controller
                             vendor: Intel Corporation
                             physical id: 2
                             bus info: pci@0000:00:02.0
                             version: 06
                             width: 64 bits
                             clock: 33MHz
                             capabilities: msi pm bus_master cap_list
                             configuration: driver=i915 latency=0
                             resources: irq:32 memory:f7800000-f7bfffff memory:d0000000-dfffffff(prefetchable) ioport:f000(size=64)
             
             
             
             
lspci -nn -s 00:02.0

            00:02.0 Display controller [0380]: Intel Corporation Xeon E3-1200 v3/4th Gen Core Processor Integrated Graphics Controller [8086:0412] (rev 06)
            
Modern hardware  https://software.intel.com/en-us/articles/opencl-drivers            
            
Legacy hardware https://software.intel.com/en-us/articles/driver-support-matrix-for-media-sdk-and-opencl

            4th Generation Core
            Haswell - Gen 7.5 graphics 
            16.4 (Media Server Studio 2015/2016)
            CentOS 7.1
            Generic kernel: 3.14.5
                
            
https://registrationcenter.intel.com/en/products/postregistration/?sn=CL5Z-TDH74TPX&EmailID=aillusions%40gmail.com&Sequence=2113383#


            SDK2016 latest release (16.4.4)

ldd --version 

uname -r

            3.10.0-229.1.2.47109.MSSr1.el7.centos.x86_64
            
lsmod | grep 'i915'

            i915                  938476  1 
            i2c_algo_bit           13413  2 i915,radeon
            drm_kms_helper         98274  2 i915,radeon
            drm                   311336  8 ttm,i915,drm_kms_helper,radeon
            i2c_core               40325  5 drm,i915,drm_kms_helper,i2c_algo_bit,radeon
            video                  19263  2 i915,asus_wmi        
            
            
find / -name "i915"

            /proc/irq/47/i915
            find: '/run/user/1000/gvfs': Permission denied
            /sys/bus/pci/drivers/i915
            /sys/kernel/debug/tracing/events/i915
            /sys/module/drm/holders/i915
            /sys/module/i915
            /sys/module/i2c_core/holders/i915
            /sys/module/video/holders/i915
            /sys/module/drm_kms_helper/holders/i915
            /sys/module/i2c_algo_bit/holders/i915
            /usr/lib/modules/3.10.0-229.1.2.47109.MSSr1.el7.centos.x86_64/kernel/drivers/gpu/drm/i915
            /usr/src/kernels/3.10.0-693.2.2.el7.x86_64.debug/drivers/gpu/drm/i915
            /usr/src/kernels/3.10.0-693.2.2.el7.x86_64.debug/include/config/drm/i915
            /usr/src/kernels/3.10.0-693.2.2.el7.x86_64/drivers/gpu/drm/i915
            /usr/src/kernels/3.10.0-693.2.2.el7.x86_64/include/config/drm/i915
            /MSS/rpmbuild/BUILD/kernel-3.10.0-229.1.2.el7/linux-3.10.0-229.1.2.47109.MSSr1.el7.centos.x86_64/drivers/gpu/drm/i915
            /MSS/rpmbuild/BUILD/kernel-3.10.0-229.1.2.el7/linux-3.10.0-229.1.2.47109.MSSr1.el7.centos.x86_64/include/config/drm/i915
            
            
echo $MFX_HOME               

            /opt/intel/mediasdk    
            
tree /etc/OpenCL

            /etc/OpenCL
            `-- vendors
                `-- intel.icd   
                
cat /etc/OpenCL/vendors/intel.icd   

            /opt/intel/opencl/libIntelOpenCL.so  
            
ldd /opt/intel/opencl/libIntelOpenCL.so

            linux-vdso.so.1 =>  (0x00007fff8c0fd000)
            libpthread.so.0 => /lib64/libpthread.so.0 (0x00007f12ffc15000)
            libdl.so.2 => /lib64/libdl.so.2 (0x00007f12ffa11000)
            librt.so.1 => /lib64/librt.so.1 (0x00007f12ff808000)
            libstdc++.so.6 => /lib64/libstdc++.so.6 (0x00007f12ff500000)
            libm.so.6 => /lib64/libm.so.6 (0x00007f12ff1fe000)
            libgcc_s.so.1 => /lib64/libgcc_s.so.1 (0x00007f12fefe7000)
            libc.so.6 => /lib64/libc.so.6 (0x00007f12fec26000)
            /lib64/ld-linux-x86-64.so.2 (0x00007f1300070000)
                                 
            
            
tree /opt/intel

            /opt/intel
            |-- common
            |   `-- mdf
            |       `-- lib64
            |           |-- igfxcmjit64.so -> libigfxcmjit64.so.4.0.0.1171
            |           |-- igfxcmrt64.so -> libigfxcmrt64.so.4.0.0.1171
            |           |-- libigfxcmjit64.so.4.0.0.1171
            |           `-- libigfxcmrt64.so.4.0.0.1171
            |-- mediasdk
            |   |-- doc
            |   |   |-- mediasdkjpeg-man.pdf
            |   |   |-- mediasdk-man.pdf
            |   |   |-- mediasdkusr-man.pdf
            |   |   `-- mediasdkvp8-man.pdf
            |   |-- include
            |   |   |-- mfxastructures.h
            |   |   |-- mfxaudio.h
            |   |   |-- mfxaudio++.h
            |   |   |-- mfxcommon.h
            |   |   |-- mfxdefs.h
            |   |   |-- mfxdispatcherprefixedfunctions.h
            |   |   |-- mfxenc.h
            |   |   |-- mfxjpeg.h
            |   |   |-- mfxla.h
            |   |   |-- mfxmvc.h
            |   |   |-- mfxpak.h
            |   |   |-- mfxplugin.h
            |   |   |-- mfxplugin++.h
            |   |   |-- mfxsession.h
            |   |   |-- mfxstructures.h
            |   |   |-- mfxvideo.h
            |   |   |-- mfxvideo++.h
            |   |   |-- mfxvp8.h
            |   |   `-- mfxvstructures.h
            |   |-- lib
            |   |   `-- lin_x64
            |   |       `-- libmfx.a
            |   |-- lib64
            |   |   |-- iHD_drv_video.so
            |   |   |-- libmfxhw64-p.so.1.17
            |   |   |-- libmfxhw64.so -> libmfxhw64-p.so.1.17
            |   |   |-- libmfxsw64-p.so.1.17
            |   |   `-- libmfxsw64.so -> libmfxsw64-p.so.1.17
            |   |-- opensource
            |   |   |-- libdrm
            |   |   |   `-- 2.4.56-47109
            |   |   |       `-- libdrm-2.4.56.tar.bz2
            |   |   |-- libva
            |   |   |   `-- 1.67.0.pre1-47109
            |   |   |       `-- libva-1.67.0.pre1.tar.bz2
            |   |   |-- mfx_dispatch
            |   |   |   |-- CMakeLists.txt
            |   |   |   |-- include
            |   |   |   |   |-- mfxaudio_exposed_functions_list.h
            |   |   |   |   |-- mfx_critical_section.h
            |   |   |   |   |-- mfx_dispatcher_defs.h
            |   |   |   |   |-- mfx_dispatcher.h
            |   |   |   |   |-- mfx_dispatcher_log.h
            |   |   |   |   |-- mfx_dxva2_device.h
            |   |   |   |   |-- mfx_exposed_functions_list.h
            |   |   |   |   |-- mfx_library_iterator.h
            |   |   |   |   |-- mfx_load_dll.h
            |   |   |   |   |-- mfx_load_plugin.h
            |   |   |   |   |-- mfx_plugin_cfg_parser.h
            |   |   |   |   |-- mfx_plugin_hive.h
            |   |   |   |   |-- mfx_vector.h
            |   |   |   |   `-- mfx_win_reg_key.h
            |   |   |   `-- src
            |   |   |       |-- main.cpp
            |   |   |       |-- mfx_critical_section.cpp
            |   |   |       |-- mfx_critical_section_linux.cpp
            |   |   |       |-- mfx_dispatcher.cpp
            |   |   |       |-- mfx_dispatcher_log.cpp
            |   |   |       |-- mfx_dxva2_device.cpp
            |   |   |       |-- mfx_function_table.cpp
            |   |   |       |-- mfx_library_iterator.cpp
            |   |   |       |-- mfx_library_iterator_linux.cpp
            |   |   |       |-- mfx_load_dll.cpp
            |   |   |       |-- mfx_load_dll_linux.cpp
            |   |   |       |-- mfx_load_plugin.cpp
            |   |   |       |-- mfx_plugin_cfg_parser.cpp
            |   |   |       |-- mfx_plugin_hive.cpp
            |   |   |       |-- mfx_plugin_hive_linux.cpp
            |   |   |       `-- mfx_win_reg_key.cpp
            |   |   |-- patches
            |   |   |   `-- kmd
            |   |   |       `-- 3.10.0
            |   |   |           `-- intel-kernel-patches.tar.bz2
            |   |   `-- readme-dispatcher-linux.pdf
            |   |-- plugins
            |   |   |-- libmfx_h264la_hw64.so
            |   |   |-- libmfx_vp8d_hw64.so
            |   |   `-- plugins.cfg
            |   `-- tools
            |       |-- drmserver
            |       |   |-- drmserver-0.0.2-1.el7.centos.src.rpm
            |       |   |-- drmserver-0.0.2-1.el7.centos.x86_64.rpm
            |       |   |-- drmserver_release_notes.pdf
            |       |   |-- libdrmclient-0.0.2-1.el7.centos.x86_64.rpm
            |       |   `-- libdrmclient-devel-0.0.2-1.el7.centos.x86_64.rpm
            |       |-- metrics_monitor
            |       |   |-- _bin
            |       |   |   |-- libcttmetrics.so
            |       |   |   `-- metrics_monitor
            |       |   |-- doc
            |       |   |   `-- metricsmon-man.pdf
            |       |   |-- include
            |       |   |   `-- cttmetrics.h
            |       |   |-- README
            |       |   `-- sample
            |       |       |-- build.sh
            |       |       |-- cttmetrics_sample.cpp
            |       |       `-- run.sh
            |       `-- tracer
            |           |-- libmfx-tracer.so
            |           |-- mfx-tracer-config
            |           `-- README
            `-- opencl
                |-- clbltfne9_img_cbk.o
                |-- clbltfne9_img_cbk.rtl
                |-- clbltfne9.rtl
                |-- clbltfnh8_img_cbk.o
                |-- clbltfnh8_img_cbk.rtl
                |-- clbltfnh8.rtl
                |-- clbltfnl9_img_cbk.o
                |-- clbltfnl9_img_cbk.rtl
                |-- clbltfnl9.rtl
                |-- clbltfnshared.rtl
                |-- igdclbif.bin
                |-- include
                |   `-- CL
                |       |-- cl_ext.h
                |       |-- cl_gl_ext.h
                |       |-- cl_gl.h
                |       |-- cl.h
                |       |-- cl.hpp
                |       |-- cl_platform.h
                |       |-- opencl.h
                |       `-- va_ext.h
                |-- libclang_compiler.so
                |-- libcl_logger.so
                |-- libcommon_clang.so
                |-- libcpu_device.so
                |-- libigdbcl.so.16 -> libigdbcl.so.16.4.0
                |-- libigdbcl.so.16.4.0
                |-- libigdfcl.so.16 -> libigdfcl.so.16.4.0
                |-- libigdfcl.so.16.4.0
                |-- libigdmcl.so.16 -> libigdmcl.so.16.4.0
                |-- libigdmcl.so.16.4.0
                |-- libigdrcl.so.16 -> libigdrcl.so.16.4.0
                |-- libigdrcl.so.16.4.0
                |-- libintelocl.so
                |-- libintelopencl64.so
                |-- libIntelOpenCL.so -> libIntelOpenCL.so.16
                |-- libIntelOpenCL.so.16 -> libIntelOpenCL.so.16.4.0
                |-- libIntelOpenCL.so.16.4.0
                |-- libmd.so
                |-- libOclCpuBackEnd.so
                |-- libOpenCL.so -> libOpenCL.so.1
                |-- libOpenCL.so.1 -> libOpenCL.so.1.2
                |-- libOpenCL.so.1.2
                |-- libtask_executor.so
                |-- libtbbmalloc.so -> libtbbmalloc.so.2
                |-- libtbbmalloc.so.2
                |-- libtbb.so -> libtbb.so.2
                |-- libtbb.so.2
                |-- __ocl_svml_e9.so
                |-- __ocl_svml_h8.so
                |-- __ocl_svml_l9.so
                |-- OpenCL.pc
                `-- opencl_.pch
            
            
ls -la /opt/intel/opencl/*libOpenCL*

            lrwxrwxrwx. 1 root root    14 Oct 16 19:14 /opt/intel/opencl/libOpenCL.so -> libOpenCL.so.1
            lrwxrwxrwx. 1 root root    16 Oct 16 19:14 /opt/intel/opencl/libOpenCL.so.1 -> libOpenCL.so.1.2
            -rwxr-xr-x. 1 root root 34968 Dec  7  2015 /opt/intel/opencl/libOpenCL.so.1.2            
                         
                         
ldd /opt/intel/opencl/libOpenCL.so

            linux-vdso.so.1 =>  (0x00007fff6e1fe000)
            libdl.so.2 => /lib64/libdl.so.2 (0x00007fd0e3c16000)
            libc.so.6 => /lib64/libc.so.6 (0x00007fd0e3855000)
            /lib64/ld-linux-x86-64.so.2 (0x00007fd0e4039000)          
            
            
            
mkdir /opt/intel/mediasdk/samples

copy /Users/mac/Downloads/Intel/MediaSamples_Linux_2016/* to /opt/intel/mediasdk

sudo yum install libX11-devel
sudo yum install mesa-libGL-devel --skip-broken 

cd /opt/intel/mediasdk/samples

perl build.pl --cmake=intel64.make.release -build
                                   
cd /opt/intel/mediasdk/samples/ocl_motion_estimation/MotionEstimation                                   