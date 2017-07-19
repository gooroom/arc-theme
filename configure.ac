AC_INIT(
    [arc-theme],
    [20161119],
    [https://github.com/horst3180/Arc-theme/issues],
    [arc-theme],
    [https://github.com/horst3180/Arc-theme],
    []
)

AC_CONFIG_AUX_DIR([build-aux])
AC_CONFIG_MACRO_DIR([m4])
AM_INIT_AUTOMAKE([no-dist-gzip dist-xz foreign])
AC_PROG_MKDIR_P

AC_PREFIX_DEFAULT(/usr)
AM_SILENT_RULES([yes])

AC_PATH_PROG([SASSC], [sassc])
if test x"$SASSC" = x; then
	AC_MSG_ERROR(['sassc' not found.])
fi


AC_CONFIG_FILES([
	src/Makefile
	Makefile
])

AC_OUTPUT
