PWD:=$(shell pwd)
TOP:=$(PWD)/../../..

# Requires that TOP be set
# Sets BUILDDIR, and BSC and BSCFLAGS if not set
include ../common.mk

.PHONY: build
build: $(BUILDDIR)
	$(BSC) -u $(BSCFLAGS) Misc.bsv

$(BUILDDIR):
	mkdir -p $@

.PHONY: clean full_clean
clean full_clean:
	@rm -f *.bi *.bo *.ba vpi_wrapper* *.info *~

