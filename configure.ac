#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT([conf-service], [0.1], [BUGREPORT@ADDRESS])
AC_CONFIG_SRCDIR([src/conf-service.in])
AC_CONFIG_AUX_DIR([build-aux])
AC_CONFIG_MACRO_DIR([m4])

AM_INIT_AUTOMAKE

# Checks for programs.

PKG_CHECK_MODULES([GUILE], [guile-2.2])
GUILE_SITE_DIR

# Checks for libraries.
GUILE_MODULE_REQUIRED([databuf])
GUILE_MODULE_REQUIRED([sqlite3])

# Checks for header files.

# Checks for typedefs, structures, and compiler characteristics.

# Checks for library functions.

AC_CONFIG_FILES([src/conf-service], [chmod +x src/conf-service])
AC_OUTPUT([Makefile
	   src/Makefile])
