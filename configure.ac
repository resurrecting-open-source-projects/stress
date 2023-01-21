AC_PREREQ([2.69])
AC_INIT([stress], [1.0.7], [https://github.com/resurrecting-open-source-projects/stress/issues])
AC_CONFIG_SRCDIR([src/stress.c])
AC_CONFIG_HEADERS([config.h])
AM_INIT_AUTOMAKE

# Checks for programs.
AC_PROG_CC
AC_PROG_INSTALL
AC_PROG_MAKE_SET

# Checks for header files.
AC_CHECK_HEADERS([stdlib.h string.h unistd.h sys/prctl.h])

# Checks for library functions.
AC_FUNC_FORK
AC_FUNC_MALLOC
AC_CHECK_FUNCS([alarm sqrt strerror])

# Special functions
AC_ARG_ENABLE([static],
               AS_HELP_STRING([--enable-static],
                              [build static library @<:@default=no@:>@]),
               [static=$enableval],
               [static=no])

if test "$static" = yes; then
        # if we're using gcc, add `-static' to LDFLAGS
        if test -n "$GCC" || test "$ac_cv_c_compiler_gnu" = "yes"; then
                STATIC_LD="-static"
                LDFLAGS="$LDFLAGS -static"
        fi
fi

AC_CONFIG_FILES([Makefile
                 src/Makefile
                 test/Makefile])
AC_OUTPUT
