# SPDX-License-Identifier: GPL-2.0-only
#
# Makefile for cnss logger
#

ifeq ($(CONFIG_CNSS_OUT_OF_TREE),y)
ccflags-y += -I$(WLAN_PLATFORM_ROOT)/inc
endif

obj-$(CONFIG_CNSS_LOGGER) += logger.o

logger-y += main.o	\
	    nl_service.o

logger-$(CONFIG_DEBUG_FS) += debugfs.o
