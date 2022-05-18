AC_PREREQ([2.57])
AC_INIT(evtest,[1.35], [https://gitlab.freedesktop.org/libevdev/evtest/issues], evtest)
AM_INIT_AUTOMAKE([foreign dist-bzip2])

AC_CONFIG_HEADERS(config.h)
AC_PROG_CC
AC_PROG_INSTALL

AC_ARG_VAR([XMLTO], [Path to xmlto command])
AC_PATH_PROG([XMLTO], [xmlto])
AC_ARG_VAR([ASCIIDOC], [Path to asciidoc command])
AC_PATH_PROG([ASCIIDOC], [asciidoc])
AM_CONDITIONAL([HAVE_DOCTOOLS], [test "x$XMLTO" != "x" && test "x$ASCIIDOC" != "x"])
if test "x$XMLTO" = "x" || test "x$ASCIIDOC" = "x"; then
	AC_MSG_WARN([xmlto or asciidoc not found - cannot create man pages without it])
fi

AC_OUTPUT([Makefile])
