
lib_LTLIBRARIES = libopenobex.la

libopenobex_la_SOURCES = \
	obex.c obex_incl.h \
	obex_main.c obex_main.h \
	obex_connect.c obex_connect.h \
	obex_header.c obex_header.h \
	obex_object.c obex_object.h \
	obex_transport.c obex_transport.h \
	obex_server.c obex_server.h \
	obex_client.c obex_client.h \
	irobex.c irobex.h \
	inobex.c inobex.h \
	btobex.c btobex.h \
	databuffer.c databuffer.h \
	irda.h irda_wrap.h \
	usbutils.c usbutils.h \
	usbobex.c usb1obex.c usbobex.h \
	bluez_compat.h \
	visibility.h defines.h debug.h

libopenobex_la_CFLAGS = @CFLAG_VISIBILITY@ @USB1_CFLAGS@

libopenobex_la_LDFLAGS = \
	-no-undefined \
	-version-info 2:0:0 \
	-export-symbols $(top_srcdir)/lib/obex.sym

libopenobex_la_LIBADD = @USB_LIBS@ @USB1_LIBS@ @EXTRA_LIBS@

INCLUDES = -I$(top_srcdir)/include

EXTRA_DIST = obex.sym win32compat.c CMakeLists.txt openobex.rc.in

MAINTAINERCLEANFILES = Makefile.in
