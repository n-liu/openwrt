#
# Copyright (C) 2010-2011 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#
include $(TOPDIR)/rules.mk

ARCH:=arm
BOARD:=omap24xx
BOARDNAME:=TI OMAP24xx
MAINTAINER:=Michael Buesch <m@bues.ch>
FEATURES:=targz squashfs jffs2_nand usb usbgadget display gpio audio broken

LINUX_VERSION:=3.3.8

define Target/Description
	TI OMAP-24xx
endef

CFLAGS:=-Os -pipe -march=armv6 -mtune=arm1136j-s -fno-caller-saves

KERNELNAME:="zImage"

include $(INCLUDE_DIR)/target.mk

$(eval $(call BuildTarget))
