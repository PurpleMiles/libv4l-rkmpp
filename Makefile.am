# Copyright (C) 2019, Fuzhou Rockchip Electronics Co., Ltd
# Released under the MIT license (see COPYING.MIT for the terms)

AUTOMAKE_OPTIONS = foreign
ACLOCAL_AMFLAGS = -I m4

libv4l2plugin_LTLIBRARIES = libv4l-rkmpp.la

noinst_HEADERS = \
	include/libv4l-rkmpp.h \
	include/libv4l-rkmpp-dec.h

libv4l_rkmpp_la_SOURCES = \
	src/libv4l-rkmpp.c \
	src/libv4l-rkmpp-dec.c

libv4l_rkmpp_la_CFLAGS = \
	$(LIBV4L2_CFLAGS) $(RKMPP_CFLAGS) -I$(top_srcdir)/include
libv4l_rkmpp_la_CPPFLAGS = $(CFLAG_VISIBILITY)
libv4l_rkmpp_la_LIBADD = $(RKMPP_LIBS)
libv4l_rkmpp_la_LDFLAGS = -avoid-version -module -shared -export-dynamic

EXTRA_DIST = COPYING
