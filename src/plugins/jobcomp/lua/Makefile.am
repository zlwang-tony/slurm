# Makefile for jobcomp/lua plugin

AUTOMAKE_OPTIONS = foreign
CLEANFILES = core.*

PLUGIN_FLAGS = -module -avoid-version --export-dynamic

AM_CPPFLAGS = -I$(top_srcdir) -I$(top_srcdir)/src/common \
	      -DDEFAULT_SCRIPT_DIR=\"$(sysconfdir)\" $(lua_CFLAGS)

if HAVE_LUA

pkglib_LTLIBRARIES = jobcomp_lua.la

# cli_filter lua plugin.
jobcomp_lua_la_SOURCES = jobcomp_lua.c
jobcomp_lua_la_LDFLAGS = $(SO_LDFLAGS) $(PLUGIN_FLAGS) $(lua_LIBS)
#jobcomp_lua_la_LIBADD = ../common/libcli_filter_common.la

else
EXTRA_jobcomp_lua_la_SOURCES = jobcomp_lua.c
endif

