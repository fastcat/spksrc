TC_NAME = syno-$(TC_ARCH)

TC_ARCH = qoriq
TC_VERS = 6.1
TC_OS_MIN_VER = 6.1-15047
TC_KERNEL = 2.6.32.12+

TC_DIST = qoriq-gcc493_glibc220_hard_qoriq-GPL
TC_EXT = txz
TC_DIST_NAME = $(TC_DIST).$(TC_EXT)
TC_DIST_SITE = https://sourceforge.net/projects/dsgpl/files/Tool%20Chain/DSM%206.1%20Tool%20Chains/PowerPC%20QorIQ%20Linux%202.6.32

TC_BASE_DIR = powerpc-e500v2-linux-gnuspe
TC_PREFIX = powerpc-e500v2-linux-gnuspe
TC_TARGET = powerpc-e500v2-linux-gnuspe

TC_CFLAGS = -I$(WORK_DIR)/$(TC_BASE_DIR)/$(TC_BASE_DIR)/sysroot/usr/include -mcpu=8548 -mhard-float -mfloat-gprs=double
TC_CPPFLAGS = -I$(WORK_DIR)/$(TC_BASE_DIR)/$(TC_BASE_DIR)/sysroot/usr/include -mcpu=8548 -mhard-float -mfloat-gprs=double
TC_CXXFLAGS = -I$(WORK_DIR)/$(TC_BASE_DIR)/$(TC_BASE_DIR)/sysroot/usr/include -mcpu=8548 -mhard-float -mfloat-gprs=double
TC_LDFLAGS = -L$(WORK_DIR)/$(TC_BASE_DIR)/$(TC_BASE_DIR)/sysroot/lib

FIX_TARGET = myFix

include ../../mk/spksrc.tc.mk

.PHONY: myFix
myFix:
	chmod -R u+w $(WORK_DIR)
	@find $(WORK_DIR)/$(TC_BASE_DIR) -type f -name '*.la' -exec sed -i -e "s|^libdir=.*$$|libdir='$(WORK_DIR)/$(TC_BASE_DIR)/$(TC_BASE_DIR)/sysroot/lib'|" {} \;
