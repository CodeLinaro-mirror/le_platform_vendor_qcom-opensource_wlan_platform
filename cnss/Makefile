# SPDX-License-Identifier: GPL-2.0-only
#
# Makefile for CNSS platform driver
#

ifeq ($(CONFIG_CNSS_OUT_OF_TREE),y)
ccflags-y += -I$(WLAN_PLATFORM_ROOT)/inc
endif

obj-$(CONFIG_CNSS)     += cnss.o
cnss-$(CONFIG_CNSS_PCI)	   += cnss_pci.o ramdump.o
cnss-$(CONFIG_CNSS_SDIO)   += cnss_sdio.o
cnss-$(CONFIG_CNSS)        += cnss_common.o
obj-$(CONFIG_CNSS_LOGGER) += logger/
