################################################
#
# Buddy Allocator Userspace
#
################################################
PK_BUDDY_USERSPACE_NAME        := buddy_userspace
PK_BUDDY_USERSPACE_VERSION     := $(CONFIG_PK_BUDDY_USERSPACE_VERSION)
PK_BUDDY_USERSPACE_SITE        := $(CONFIG_PK_BUDDY_USERSPACE_URL)
PK_BUDDY_USERSPACE_GITHUB      := $(CONFIG_PK_BUDDY_USERSPACE_GITHUB)
PK_BUDDY_USERSPACE_SUBNAME     :=
PK_BUDDY_USERSPACE_BUILDARCH   := $(CONFIG_PK_BUDDY_USERSPACE_BUILDARCH)
PK_BUDDY_USERSPACE_DIR         := $(srctree)/package/buddy/buddy_userspace
PK_BUDDY_USERSPACE_PATCH       := $(PK_BUDDY_USERSPACE_DIR)/patch
PK_BUDDY_USERSPACE_BSBIT       := buddy_userspace-$(PK_BUDDY_USERSPACE_VERSION).bsbit
PK_BUDDY_USERSPACE_OUT         :=
PK_BUDDY_USERSPACE_SCRIPTS     := $(srctree)/scripts/package/package-app.sh
PK_BUDDY_USERSPACE_TAR         := $(CONFIG_PK_BUDDY_USERSPACE_TAR)
PK_BUDDY_USERSPACE_PACKAGE     :=
PK_BUDDY_USERSPACE_CONFIG      := $(CONFIG_PK_BUDDY_USERSPACE_CONFIG)
SUB_TARGET                  += $(PK_BUDDY_USERSPACE_DIR)/build

PK_BUDDY_USERSPACE_sh = $(CONFIG_SHELL) $(PK_BUDDY_USERSPACE_SCRIPTS) \
                 $1X \
                 $(PK_BUDDY_USERSPACE_NAME)X \
                 $(PK_BUDDY_USERSPACE_VERSION)X \
                 $(PK_BUDDY_USERSPACE_SITE)X \
                 $(PK_BUDDY_USERSPACE_GITHUB)X \
                 $(PK_BUDDY_USERSPACE_PATCH)X \
                 $(CONFIG_LINUX_KERNEL_VERSION)X \
	         $(CONFIG_MAIN_PROJ_NAME)X \
                 $(PK_BUDDY_USERSPACE_TAR)X \
                 $(CONFIG_LINUX_KERNEL_CROSS_COMPILE)X \
                 $(PK_BUDDY_USERSPACE_SUBNAME)X \
                 $(CONFIG_PK_BUDDY_USERSPACE_CONFIG)X \
                 $(CONFIG_PK_BUDDY_USERSPACE_LIBPATH)X \
                 $(CONFIG_PK_BUDDY_USERSPACE_CPPFLAGS)X \
                 $(CONFIG_PK_BUDDY_USERSPACE_DPKCONFIG)X \
                 $(CONFIG_PK_BUDDY_USERSPACE_CFLAGS)X \
                 $(CONFIG_PK_BUDDY_USERSPACE_LDFLAGS)X \
                 $(CONFIG_PK_BUDDY_USERSPACE_CXXFLAGS)X \
                 $(CONFIG_PK_BUDDY_USERSPACE_ASFLAGS)X \
                 $(PK_BUDDY_USERSPACE_BSBIT)X \
                 $(PK_BUDDY_USERSPACE_BUILDARCH)X \
		 $(PK_BUDDY_USERSPACE_CSRCFILE)X \
                 $(CONFIG_PK_BUDDY_USERSPACE_SRCFILE)X \
                 $(CONFIG_PK_BUDDY_USERSPACE_CSRCFILE)

$(PK_BUDDY_USERSPACE_DIR)/build: FORCE
	$(Q)$(call PK_BUDDY_USERSPACE_sh,$(srctree))
