# Copyright 2011-2017 Rajesh Jayaprakash <rajesh.jayaprakash@gmail.com>

# This file is part of pLisp.

# pLisp is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.

# pLisp is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.

# You should have received a copy of the GNU General Public License
# along with pLisp.  If not, see <http://www.gnu.org/licenses/>.

AC_INIT([plisp], [0.1.4], [rajesh.jayaprakash@gamil.com], [plisp], [https://github.com/shikantaza/plisp])
AC_PREREQ([2.68])
AC_CONFIG_SRCDIR([src/main.c])
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_AUX_DIR([build-aux])

AC_CONFIG_MACRO_DIR([m4])

AM_INIT_AUTOMAKE([1.11 -Wall subdir-objects])
AC_CONFIG_FILES([Makefile])
AC_PROG_CC
AC_PROG_LEX
AC_PROG_YACC
#AC_PROG_RANLIB
AM_PROG_CC_C_O
# Put various checks and such here.

AC_SEARCH_LIBS([dlopen], [dl], [], [])

PKG_CHECK_MODULES([gtk], [gtk+-3.0 >= 3.4.2])
PKG_CHECK_MODULES([gtksourceview], [gtksourceview-3.0 >= 3.4.2])
PKG_CHECK_MODULES([libffi], [libffi >= 3.0.11])

LT_INIT

AC_OUTPUT
