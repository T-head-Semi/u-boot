# SPDX-License-Identifier: GPL-2.0+

dtb-$(CONFIG_TARGET_AX25_AE350) += ae350_32.dtb ae350_64.dtb
dtb-$(CONFIG_TARGET_SIFIVE_FU540) += hifive-unleashed-a00.dtb
dtb-$(CONFIG_TARGET_ICE_C910) += ice-c910.dtb
dtb-$(CONFIG_TARGET_ICE_C910) += ice-c910-uart0.dtb
dtb-$(CONFIG_TARGET_LIGHT_EVB_MPW_C910) += light-evb-mpw-c910.dtb
dtb-$(CONFIG_TARGET_LIGHT_FPGA_FM_C910) += light-fpga-fm-c910.dtb

targets += $(dtb-y)

DTC_FLAGS += -R 4 -p 0x1000

PHONY += dtbs
dtbs: $(addprefix $(obj)/, $(dtb-y))
	@:

clean-files := *.dtb
