TC_NAME = syno-$(TC_ARCH)

TC_ARCH = bromolow
TC_VERS = 4.3
TC_FIRMWARE = 3.1-1594

TC_DIST = gcc420_glibc236_x64_bromolow-GPL
TC_EXT = tgz
TC_DIST_NAME = $(TC_DIST).$(TC_EXT)
TC_DIST_SITE = https://sourceforge.net/projects/dsgpl/files/Tool%20Chain/DSM%204.3%20Tool%20Chains/Intel%20x86%20Linux%203.2.40%20%28Bromolow%29

TC_BASE_DIR = x86_64-linux-gnu
TC_PREFIX = x86_64-linux-gnu
TC_TARGET = x86_64-linux-gnu

TC_CFLAGS = -I$(WORK_DIR)/$(TC_BASE_DIR)/$(TC_BASE_DIR)/sys-root/usr/include
TC_CPPFLAGS = -I$(WORK_DIR)/$(TC_BASE_DIR)/$(TC_BASE_DIR)/sys-root/usr/include
TC_CXXFLAGS = -I$(WORK_DIR)/$(TC_BASE_DIR)/$(TC_BASE_DIR)/sys-root/usr/include
TC_LDFLAGS = -L$(WORK_DIR)/$(TC_BASE_DIR)/$(TC_BASE_DIR)/sys-root/lib

include ../../mk/spksrc.tc.mk
