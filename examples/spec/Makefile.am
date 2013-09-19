AM_CFLAGS = -Wall

if DEBUG
AM_CFLAGS += -g
else
AM_CFLAGS += -DNDEBUG -O2
endif

if PROFILE
AM_CFLAGS += -pg
endif

if COVERAGE
AM_CFLAGS += -fprofile-arcs -ftest-coverage
endif

AM_CPPFLAGS	=	-I$(top_srcdir)/inc

TESTS	=	spec
check_PROGRAMS	=	$(TESTS)
spec_SOURCES	=	spec_runner.c cspec_output_junit_xml_spec.c array_spec.c
spec_LDADD	=	../../src/libcspec.a
