include $(top_srcdir)/Makefile.decl

all-local: check-local

if HAVE_UMOCKDEV

noinst_PROGRAMS = test-enumerator-filter
TEST_PROGS += $(noinst_PROGRAMS)

test_enumerator_filter_SOURCES = test-enumerator-filter.c
test_enumerator_filter_CFLAGS = $(UMOCKDEV_CFLAGS) -I$(top_srcdir)
test_enumerator_filter_LDADD = $(UMOCKDEV_LIBS) $(top_builddir)/libgudev-1.0.la

endif

EXTRA_DIST = test-enumerator-filter.c
