#
# Makefile.am for core/agent-probe/src
#

AM_CXXFLAGS = -DY2LOG=\"agent-probe\" $(HWINFO_CFLAGS)

plugin_LTLIBRARIES = libpy2ag_hwprobe.la
noinst_LTLIBRARIES = liby2ag_hwprobe.la

INCLUDES = -I$(includedir)

liby2ag_hwprobe_la_SOURCES =	\
	HwProbe.cc HwProbe.h	\
	HwParse.cc

liby2ag_hwprobe_la_LDFLAGS = -version-info 2:0
liby2ag_hwprobe_la_LIBADD = @AGENT_LIBADD@ $(HWINFO_LIBS)

libpy2ag_hwprobe_la_SOURCES =				\
	$(liby2ag_hwprobe_la_SOURCES)			\
	Y2CCHwProbe.cc
libpy2ag_hwprobe_la_LDFLAGS = -version-info 2:0
libpy2ag_hwprobe_la_LIBADD = @AGENT_LIBADD@ $(HWINFO_LIBS)

