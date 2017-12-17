AC_PREREQ([2.69])
AC_INIT([unfrak-systemd-network], [1.01], [mrsam@courier-mta.com])

# Checks for programs.
AM_INIT_AUTOMAKE

# Checks for libraries.

# Checks for header files.

# Checks for typedefs, structures, and compiler characteristics.

# Checks for library functions.

AC_ARG_WITH(unitdir, [--with-unitdir    Specifies systemd unit directory],
           [ unitdir="$withval" ],
	   [ unitdir='$prefix/lib/systemd' ])

test "x$prefix" = xNONE && prefix=$ac_default_prefix
test "x$exec_prefix" = xNONE && exec_prefix="${prefix}"

eval "sysconfdir=$sysconfdir"
eval "sbindir=$sbindir"
eval "unitdir=$unitdir"

AC_SUBST(unitdir)

AC_CONFIG_FILES([
     Makefile
     unfrak-systemd-network.spec
     unfrak-systemd-network.service
])
AC_OUTPUT
