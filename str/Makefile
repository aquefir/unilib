##############################################################################
##                            Hinterlib™ strings                            ##
##                                                                          ##
##                      Copyright © 2019-2021 Aquefir.                      ##
##                       Released under BSD-2-Clause.                       ##
##############################################################################

ifeq ($(strip $(AQ)),)
$(error "AQ was not found in your environment. You need to install the Slick Makefiles from github.com/aquefir/slick to continue.")
endif

include $(AQ)/lib/slick/base.mk

PROJECT := uni_str

# put a ‘1’ for the desired target types to compile
SOFILE :=
AFILE  := 1

# space-separated path list for #includes
# <system> includes
INCLUDES := include ../decl/include ../err/include ../himem/include \
	../log/include
# "local" includes
INCLUDEL := src

# space-separated library name list
LIBS    := uni_log uni_err uni_himem
LIBDIRS :=

# frameworks (macOS target only)
FWORKS :=

# ‘3P’ are in-tree 3rd-party dependencies
# 3PLIBDIR is the base directory
# 3PLIBS is the folder names in the base directory for each library
3PLIBDIR :=
3PLIBS   :=

# sources
SFILES    :=
CFILES    := \
	src/str.c \
	src/utf8.c
CPPFILES  :=
PUBHFILES := \
	include/uni/str.h \
	include/uni/utf8.h
PRVHFILES := \
	src/str.h \
	src/utf8.h

# test suite sources
TES_CFILES    := \
	src/str.tes.c \
	src/utf8.tes.c
TES_CPPFILES  :=
TES_PUBHFILES :=
TES_PRVHFILES :=

# this defines all our usual targets
include $(AQ)/lib/slick/targets.mk
