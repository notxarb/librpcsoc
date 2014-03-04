# rebuild: autoreconf -fvi 

AC_PREREQ(2.61)

AC_INIT([librpcsoc], [1])
AM_INIT_AUTOMAKE([foreign subdir-objects])
AC_CONFIG_SRCDIR([src])
AC_CONFIG_MACRO_DIR([m4])

AC_PROG_CC
AC_PROG_LIBTOOL

AC_CHECK_LIB(nsl, svc_dg_enablecache,
  [],
  [AC_MSG_ERROR([nsl libraries not found.])]
)

AC_CHECK_LIB(socket, getnameinfo,
  [],
  [AC_MSG_ERROR([socket libraries not found.])]
)

AC_CHECK_LIB(c, pthread_spin_unlock,
  [],
  [AC_MSG_ERROR([c libraries not found.])]
)

AC_OUTPUT(Makefile src/Makefile)
