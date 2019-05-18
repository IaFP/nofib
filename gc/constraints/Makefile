TOP = ../..
include $(TOP)/mk/boilerplate.mk

FAST_OPTS = 7
# NORM_OPTS should probably be 8 or 9
NORM_OPTS = 10
SLOW_OPTS = 11

ifeq "$(HEAP)" "LARGE"
PROG_ARGS += +RTS -H330m -RTS
endif
ifeq "$(HEAP)" "OLD"
PROG_ARGS += +RTS -H10m -RTS
endif

include $(TOP)/mk/target.mk
