# SPDX-License-Identifier: GPL-2.0-only
#
# Makefile for CNSS platform driver
#
MODNAME := cnss
ifeq ($(CONFIG_CNSS_OUT_OF_TREE),y)
ccflags-y += -I$(WLAN_PLATFORM_ROOT)/inc
endif

obj-$(CONFIG_CNSS)     += $(MODNAME).o
$(MODNAME)-$(CONFIG_CNSS_PCI)	   += cnss_pci.o ramdump.o
$(MODNAME)-$(CONFIG_CNSS_SDIO)   += cnss_sdio.o ramdump.o
$(MODNAME)-$(CONFIG_CNSS)        += cnss_common.o
obj-$(CONFIG_CNSS_LOGGER) += logger/
