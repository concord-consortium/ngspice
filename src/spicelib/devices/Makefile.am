## Process this file with automake to produce Makefile.in

SUBDIRS = \
	bjt	\
	cap	\
	dio	\
	ind	\
	isrc	\
	res	\
	sw	\
	vsrc	\
	@VLADEVDIR@

if NDEV_WANTED
SUBDIRS += ndev
endif

if NUMDEV_WANTED
SUBDIRS += nbjt nbjt2 numd  numd2 numos
endif

DIST_SUBDIRS = \
	@VLADEVDIR@ \
	bjt	\
	cap	\
	dio	\
	ind	\
	isrc	\
	res	\
	soi3	\
	sw


noinst_LTLIBRARIES = libdev.la

libdev_la_SOURCES =	\
	dev.c		\
	dev.h		\
	devsup.c	\
	cktaccept.c	\
	cktaccept.h	\
	cktask.c	\
	cktbindnode.c	\
	cktcrte.c	\
	cktfinddev.c	\
	cktinit.c	\
	cktsoachk.c	\
	limit.c

EXTRA_DIST = @NOTVLADEVDIR@

AM_CPPFLAGS = @AM_CPPFLAGS@ -I$(top_srcdir)/src/include -I$(top_srcdir)/src/spicelib/devices
AM_CFLAGS = $(STATIC)

MAINTAINERCLEANFILES = Makefile.in
