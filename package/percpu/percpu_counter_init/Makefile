################################################
#
# percpu_counter_init
#
################################################
PK_PERCPU_COUNTER_INIT_NAME        := percpu_counter_init
PK_PERCPU_COUNTER_INIT_VERSION     := $(CONFIG_PK_PERCPU_COUNTER_INIT_VERSION)
PK_PERCPU_COUNTER_INIT_SITE        := $(CONFIG_PK_PERCPU_COUNTER_INIT_URL)
PK_PERCPU_COUNTER_INIT_GITHUB      := $(CONFIG_PK_PERCPU_COUNTER_INIT_GITHUB)
PK_PERCPU_COUNTER_INIT_SUBNAME     :=
PK_PERCPU_COUNTER_INIT_BUILDARCH   := $(CONFIG_PK_PERCPU_COUNTER_INIT_BUILDARCH)
PK_PERCPU_COUNTER_INIT_DIR         := $(srctree)/package/percpu/percpu_counter_init
PK_PERCPU_COUNTER_INIT_PATCH       := $(PK_PERCPU_COUNTER_INIT_DIR)/patch
PK_PERCPU_COUNTER_INIT_BSBIT       := percpu_counter_init-$(PK_PERCPU_COUNTER_INIT_VERSION).bsbit
PK_PERCPU_COUNTER_INIT_OUT         :=
PK_PERCPU_COUNTER_INIT_SCRIPTS     := $(srctree)/scripts/package/package-module.sh
PK_PERCPU_COUNTER_INIT_TAR         := $(CONFIG_PK_PERCPU_COUNTER_INIT_TAR)
PK_PERCPU_COUNTER_INIT_PACKAGE     :=
PK_PERCPU_COUNTER_INIT_CONFIG      := $(CONFIG_PK_PERCPU_COUNTER_INIT_CONFIG)
SUB_TARGET                  += $(PK_PERCPU_COUNTER_INIT_DIR)/build

PK_PERCPU_COUNTER_INIT_sh = $(CONFIG_SHELL) $(PK_PERCPU_COUNTER_INIT_SCRIPTS) \
                 $1X \
                 $(PK_PERCPU_COUNTER_INIT_NAME)X \
                 $(PK_PERCPU_COUNTER_INIT_VERSION)X \
                 $(PK_PERCPU_COUNTER_INIT_SITE)X \
                 $(PK_PERCPU_COUNTER_INIT_GITHUB)X \
                 $(PK_PERCPU_COUNTER_INIT_PATCH)X \
                 $(CONFIG_LINUX_KERNEL_VERSION)X \
	         $(CONFIG_MAIN_PROJ_NAME)X \
                 $(PK_PERCPU_COUNTER_INIT_TAR)X \
                 $(CONFIG_LINUX_KERNEL_CROSS_COMPILE)X \
                 $(PK_PERCPU_COUNTER_INIT_SUBNAME)X \
                 $(CONFIG_PK_PERCPU_COUNTER_INIT_CONFIG)X \
                 $(CONFIG_PK_PERCPU_COUNTER_INIT_LIBPATH)X \
                 $(CONFIG_PK_PERCPU_COUNTER_INIT_CPPFLAGS)X \
                 $(CONFIG_PK_PERCPU_COUNTER_INIT_DPKCONFIG)X \
                 $(CONFIG_PK_PERCPU_COUNTER_INIT_CFLAGS)X \
                 $(CONFIG_PK_PERCPU_COUNTER_INIT_LDFLAGS)X \
                 $(CONFIG_PK_PERCPU_COUNTER_INIT_CXXFLAGS)X \
                 $(CONFIG_PK_PERCPU_COUNTER_INIT_ASFLAGS)X \
                 $(PK_PERCPU_COUNTER_INIT_BSBIT)X \
                 $(PK_PERCPU_COUNTER_INIT_BUILDARCH)X \
		 $(PK_PERCPU_COUNTER_INIT_CSRCFILE)X \
                 $(CONFIG_PK_PERCPU_COUNTER_INIT_SRCFILE)X \
                 $(CONFIG_PK_PERCPU_COUNTER_INIT_CSRCFILE)

$(PK_PERCPU_COUNTER_INIT_DIR)/build: FORCE
	$(Q)$(call PK_PERCPU_COUNTER_INIT_sh,$(srctree))
