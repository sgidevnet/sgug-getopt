AC_PREREQ(2.65)
AC_INIT([sgug-getopt],
        [0.1.0],
        [daniel.hams@gmail.com])

AC_SUBST(ACLOCAL_AMFLAGS, "-I macros")

AC_CONFIG_SRCDIR(src)
AC_CONFIG_MACRO_DIR(macros)
AC_CONFIG_HEADERS(config.h)
AM_INIT_AUTOMAKE([1.9 foreign subdir-objects])

ABI_VERSION=0.1
AC_SUBST(ABI_VERSION)
AC_DEFINE_UNQUOTED(ABI_VERSION, "$ABI_VERSION", [ABI version of the package])
PACKAGE_SUFFIX="-${ABI_VERSION}"
AC_SUBST(PACKAGE_SUFFIX)
AC_DEFINE_UNQUOTED(PACKAGE_SUFFIX, "$PACKAGE_SUFFIX", [Suffix of the package])

AC_STDC_HEADERS
AC_PROG_CC
AC_PROG_CXX
AC_PROG_LIBTOOL
PKG_PROG_PKG_CONFIG

AC_LANG([C])

AM_PROG_CC_C_O
AC_PROG_MKDIR_P
AC_PROG_CC_STDC
AC_PROG_YACC
AC_CANONICAL_HOST
AC_C_CONST
AC_C_VOLATILE
AC_C_BIGENDIAN

AC_SYS_LARGEFILE
AC_HEADER_ASSERT
AC_STRUCT_TIMEZONE

AM_GNU_GETTEXT_VERSION([0.18.3])
AM_GNU_GETTEXT([external])

AC_CHECK_HEADERS([ \
	asm/io.h \
	err.h \
	errno.h \
	fcntl.h \
	getopt.h \
	inttypes.h \
	lastlog.h \
	libutil.h \
	locale.h \
	mntent.h \
	net/if.h \
	net/if_dl.h \
	netinet/in.h \
	paths.h \
	pty.h \
	security/pam_appl.h \
	stdint.h \
	stdio_ext.h \
	stdlib.h \
	endian.h \
	byteswap.h \
	sys/endian.h \
	sys/disk.h \
	sys/disklabel.h \
	sys/file.h \
	sys/io.h \
	sys/ioccom.h \
	sys/ioctl.h \
	sys/mkdev.h \
	sys/mount.h \
	sys/param.h \
	sys/prctl.h \
	sys/resource.h \
	sys/signalfd.h \
	sys/socket.h \
	sys/sockio.h \
	sys/stat.h \
	sys/sysmacros.h \
	sys/swap.h \
	sys/syscall.h \
	sys/time.h \
	sys/timex.h \
	sys/ttydefaults.h \
	sys/types.h \
	sys/ucred.h \
	sys/un.h \
	unistd.h \
	shadow.h \
	utmp.h \
	utmpx.h \
])

AC_CHECK_FUNCS([ \
	clearenv \
	__fpurge \
	fpurge \
	__fpending \
	secure_getenv \
	__secure_getenv \
	eaccess \
	err \
	errx \
	explicit_bzero \
	fsync \
	utimensat \
	getdomainname \
	getdtablesize \
	getexecname \
	getmntinfo \
	getrandom \
	getrlimit \
	getsgnam \
	inotify_init \
	jrand48 \
	lchown \
	llseek \
	lseek64 \
	mempcpy \
	mkostemp \
	nanosleep \
	ntp_gettime \
	personality \
	posix_fadvise \
	prctl \
	qsort_r \
	rpmatch \
	scandirat \
	setprogname \
	setresgid \
	setresuid \
	sched_setattr \
	sched_setscheduler \
	sigqueue \
	srandom \
	strnchr \
	strndup \
	strnlen \
	sysconf \
	sysinfo \
	timegm \
	usleep \
	vwarnx \
	warn \
	warnx \
])
AC_FUNC_FSEEKO

LIBDICL_VERSION=0.1.19
AC_SUBST(LIBDICL_VERSION)

DICL_PACKAGE_DEPENDENCY_LIST="libdicl-0.1 >= $LIBDICL_VERSION"
AC_DEFINE_UNQUOTED(DICL_PACKAGE_DEPENDENCY_LIST, "$DICL_PACKAGE_DEPENDENCY_LIST", [Dicl package dependency list])

PKG_CHECK_MODULES([DICL_DEPS], [$DICL_PACKAGE_DEPENDENCY_LIST])

AC_OUTPUT([Makefile
src/Makefile
src/sgug-getopt/Makefile])
