
if APPS
noinst_LIBRARIES = libircp.a

libircp_a_SOURCES = \
	ircp_client.c ircp_client.h \
	ircp_server.c ircp_server.h \
	ircp_io.c ircp_io.h \
	dirtraverse.c dirtraverse.h \
	debug.h ircp.h

bin_PROGRAMS = ircp 

AM_CFLAGS = @OPENOBEX_CFLAGS@

LDADD = libircp.a $(top_builddir)/lib/libopenobex.la

INCLUDES = -I$(top_srcdir)/include
endif

EXTRA_DIST = CMakeLists.txt

MAINTAINERCLEANFILES = Makefile.in
