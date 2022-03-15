CONTIKI_PROJECT = hello-world
all: $(CONTIKI_PROJECT)

CONTIKI = ../..

# Enable TI Over-the-Air Download (OAD)
MAKE_WITH_TI_OAD ?= 1

CFLAGS += -Wno-missing-braces

ifeq ($(MAKE_WITH_TI_OAD),1)
  MODULES += $(CONTIKI_NG_SERVICES_DIR)/ti-oad
endif

include $(CONTIKI)/Makefile.include
