#-------------------------------------------------------------------------
#
# Makefile for src/test/authentication
#
# Portions Copyright (c) 1996-2018, PostgreSQL Global Development Group
# Portions Copyright (c) 1994, Regents of the University of California
#
# src/test/authentication/Makefile
#
#-------------------------------------------------------------------------

subdir = src/test/authentication
top_builddir = ../../..
include $(top_builddir)/src/Makefile.global

check:
	$(prove_check)
checkdma:
	$(prove_checkdma)

installcheck:
	$(prove_installcheck)

clean distclean maintainer-clean:
	rm -rf tmp_check
