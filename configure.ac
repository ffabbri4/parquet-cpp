AC_PREREQ([2.69])
AC_INIT([parquet-cpp], [0.1], [none])
AM_INIT_AUTOMAKE([-Wall -Werror foreign subdir-objects])

AC_CONFIG_SRCDIR([src/parquet.cc])
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_MACRO_DIR([m4])

# Checks for programs.
AC_PROG_CXX
AC_PROG_CC
AC_PROG_INSTALL
AC_PROG_LN_S
AC_PROG_MAKE_SET
AM_PROG_AR

# Checks for libraries.
LT_INIT
AX_BOOST_BASE([1.33.1])
AX_BOOST_THREAD
AX_BOOST_REGEX
AX_BOOST_SYSTEM
AX_BOOST_FILESYSTEM
PKG_CHECK_MODULES([THRIFT],[thrift])
PKG_CHECK_MODULES([LZ4],[liblz4])
AC_SEARCH_LIBS([LZ4_decompress_safe],[lz4],[],[AC_MSG_ERROR([LZ4 library not found])])
AC_SEARCH_LIBS([snappy_uncompress],[snappy],[],[AC_MSG_ERROR([snappy library not found])])
AC_SEARCH_LIBS([TLSv1_2_method],[ssl],[],[AC_MSG_ERROR([ssl library not found])])


# Checks for header files.
AC_CHECK_HEADERS([stdlib.h string.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_CHECK_HEADER_STDBOOL
AC_C_INLINE
AC_TYPE_INT16_T
AC_TYPE_INT32_T
AC_TYPE_INT64_T
AC_TYPE_INT8_T
AC_TYPE_SIZE_T
AC_TYPE_UINT16_T
AC_TYPE_UINT32_T
AC_TYPE_UINT64_T
AC_TYPE_UINT8_T

# Checks for library functions.
AC_FUNC_MALLOC
AC_CHECK_FUNCS([clock_gettime floor memmove])

AC_CONFIG_FILES([Makefile src/Makefile example/Makefile generated/Makefile])

AC_OUTPUT
