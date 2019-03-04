

# Avnet Xilinx AES-ULTRA96 Development
Author: **[Dengxue Yan](https://sites.google.com/site/ydengxue/)**
****

This *zynqmp_fsbl.elf* enables serial port console for Avnet Ultra96 board's u-boot and OS.
It modified the pin mux of uart1 (J6) based on the out of box BSP.

Use this *zynqmp_fsbl.elf* to replace the original *fsbl.elf* or *zynqmp_fsbl.elf*, and then regenerate *BOOT.BIN*:

*petalinux-package --boot --fsbl components/plnx_workspace/fsbl/fsbl/Release/fsbl.elf --fpga hardware/xilinx-ultra96-reva-2018.2/xilinx-ultra96-reva-2018.2.runs/impl_1/design_1_wrapper.bit --pmufw components/plnx_workspace/pmu-firmware/pmu-firmware/Release/pmu-firmware.elf --u-boot*

Email: Dengxue.Yan@dxyan.org
