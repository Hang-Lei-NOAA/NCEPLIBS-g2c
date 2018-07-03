## Put version control id tag in output configure script
AC_REVISION($Id: configure.ac 33161 2018-07-02 22:39:31Z dusan.jovic@noaa.gov $)

## Initialize autoconf
AC_INIT([nceplibs g2c],[v1.6.0],[ncep.list.emc.nceplibs.support@noaa.gov],[g2c])

# Output info for user
AC_MSG_NOTICE([AC_PACKAGE_NAME AC_PACKAGE_VERSION])

# Check for existence of unique file before proceeding
AC_CONFIG_SRCDIR([sorc/grib2.h])

# Define the configuration files
AC_CONFIG_FILES([Makefile sorc/Makefile])

# Check for programs
AC_PROG_CC(icc gcc xlc pgcc)
AC_PROG_INSTALL
AC_PROG_RANLIB
AC_CHECK_TOOL([AR], ar)

# ...Set defaults for ARFLAGS since there is no autoconf macro
test -n "$ARFLAGS" || ARFLAGS="crvs"
AC_SUBST(ARFLAGS)

AC_OUTPUT
