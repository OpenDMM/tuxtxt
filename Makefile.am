installdir = $(CONFIGDIR)/tuxtxt

SUBDIRS = font python

AM_CPPFLAGS = \
	@FREETYPE_CFLAGS@ \
	-funsigned-char \
	-I$(top_srcdir)/include \
	-I$(prefix)/$(includedir)/tuxbox/tuxtxt 

bin_PROGRAMS = tuxtxt
tuxtxt_LDADD = -lpthread -lz \
	@FREETYPE_LIBS@ \
	@TUXTXT_LIBS@

tuxtxt_SOURCES = tuxtxt.c

install_DATA = tuxtxt2.conf
