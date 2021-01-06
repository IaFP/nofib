TOP = ../..

include $(TOP)/mk/boilerplate.mk

FAST_OPTS = 8 100
NORM_OPTS = 8 3000
SLOW_OPTS = 8 5000

ifeq "$(HEAP)" "LARGE"
PROG_ARGS += +RTS -H256m -RTS
endif
ifeq "$(HEAP)" "OLD"
PROG_ARGS += +RTS -H30m -RTS
endif

include $(TOP)/mk/target.mk
