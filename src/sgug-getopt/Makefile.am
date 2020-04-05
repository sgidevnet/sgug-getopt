NULL=

bin_PROGRAMS=getopt

getopt_SOURCES=				\
	c.h				\
	closestream.h			\
	nls.h				\
	xalloc.h			\
	getopt.c			\
	$(NULL)

AM_CFLAGS=				\
	$(DICL_DEPS_CFLAGS)		\
	$(NULL)

getopt_LDADD=				\
	$(DICL_DEPS_LIBS)		\
	$(LTLIBINTL)			\
	$(NULL)

CLEANFILES=						\
	.libs						\
	$(NULL)
