noinst_LTLIBRARIES = libloader.la

INCLUDES = $(XORG_INCS) -I$(srcdir)/../parser -I$(top_srcdir)/miext/cw \
	   -I$(srcdir)/../ddc -I$(srcdir)/../i2c -I$(srcdir)/../modes \
	   -I$(srcdir)/../ramdac

#AM_LDFLAGS = -r
AM_CFLAGS = $(DIX_CFLAGS) $(XORG_CFLAGS)

EXTRA_DIST = \
	loader.h \
	loaderProcs.h

libloader_la_SOURCES = \
	loader.c \
	loaderProcs.h \
	loadext.c \
        loadmod.c \
	os.c

libloader_la_LIBADD = $(DLOPEN_LIBS)
