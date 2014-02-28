# -*- mode: Makefile; tab-width: 4; indent-tabs-mode: 1; st-rulers: [70] -*-
# vim: ts=8 sw=8 ft=Makefile noet

RPCSOC_LIBRARY_VERSION=1:0:0

lib_LTLIBRARIES = librpcsoc.la

librpcsoc_la_SOURCES = clnt_tcp.c clnt_udp.c get_myaddress.c getrpcport.c rtime.c svc_tcp.c svc_udp.c

librpcsoc_la_LDFLAGS = -version-info $(RPCSOC_LIBRARY_VERSION)

