# Makefile.am for cons_common

AUTOMAKE_OPTIONS = foreign
CLEANFILES = core.*

AM_CPPFLAGS = -I$(top_srcdir)

# making a .la

noinst_LTLIBRARIES = libcons_common.la
libcons_common_la_SOURCES =    \
	cons_common.c cons_common.h \
	core_array.c core_array.h \
	dist_tasks.c dist_tasks.h \
	job_resources.c job_resources.h \
	job_test.c job_test.h \
	node_data.c node_data.h \
	part_data.c part_data.h
