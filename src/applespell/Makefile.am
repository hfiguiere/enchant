target_lib = libenchant_applespell.la

INCLUDES=-I$(top_srcdir)/src $(ENCHANT_CFLAGS) $(CC_WARN_CFLAGS) -DXP_TARGET_COCOA -xobjective-c -D_ENCHANT_BUILD=1

applespell_LTLIBRARIES = $(target_lib)
applespelldir= $(libdir)/enchant

libenchant_applespell_la_LIBADD= $(ENCHANT_LIBS) -lobjc $(top_builddir)/src/libenchant.la
libenchant_applespell_la_LDFLAGS = -module -avoid-version -no-undefined -framework Cocoa
libenchant_applespell_la_SOURCES = applespell_provider.m
libenchant_applespell_la_LIBTOOLFLAGS = --tag=CC

libenchant_applespell_lalibdir=$(libdir)/enchant
