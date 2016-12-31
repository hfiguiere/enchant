AM_CPPFLAGS=-I$(top_srcdir)/src $(ENCHANT_CFLAGS) $(UNITTESTPP_CFLAGS)

DEPS= $(top_builddir)/src/libenchant.la
ldadd= $(top_builddir)/src/libenchant.la  $(ENCHANT_LIBS)

if WITH_CXX
cxx_progs = main
else
cxx_progs =
endif

noinst_PROGRAMS = $(cxx_progs)

main_SOURCES = main.cpp
main_LDFLAGS =
main_DEPENDENCIES = $(DEPS)
main_LDADD = $(ldadd) $(UNITTESTPP_LIBS)
