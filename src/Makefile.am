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

lib_LIBRARIES	=	libcspec.a
libcspec_a_SOURCES	=	\
	cspec_output_header.c \
	cspec_output_verbose.c \
	cspec_output_xml.c \
	cspec_runner.c \
	cspec_config.c \
	cspec_output_unit.c \
	cspec_private.c \
	cspec_output.c \
	array.c \
	cspec_output_junit_xml.c
