##############################################################################
##                       Hinterlib™ base declarations                       ##
##                                                                          ##
##                      Copyright © 2019-2021 Aquefir.                      ##
##                       Released under BSD-2-Clause.                       ##
##############################################################################

ifeq ($(strip $(AQ)),)
$(error "AQ was not found in your environment. You need to install the Slick Makefiles from github.com/aquefir/slick to continue.")
endif

include $(AQ)/lib/slick/base.mk

PROJECT := uni_decl

# put a ‘1’ for the desired target types to compile
SOFILE :=
AFILE  :=

# space-separated path list for #includes
# <system> includes
INCLUDES := include
# "local" includes
INCLUDEL := src

# space-separated library name list
LIBS    :=
LIBDIRS :=

# frameworks (macOS target only)
FWORKS :=

# ‘3P’ are in-tree 3rd-party dependencies
# 3PLIBDIR is the base directory
# 3PLIBS is the folder names in the base directory for each library
3PLIBDIR := 3rdparty
3PLIBS   := tes

# sources
SFILES    :=
CFILES    :=
CPPFILES  :=
PUBHFILES := \
	include/uni/types/bound.h \
	include/uni/types/complexf.h \
	include/uni/types/complexi.h \
	include/uni/types/float.h \
	include/uni/types/geo.h \
	include/uni/types/int.h \
	include/uni/types/mathprim.h \
	include/uni/types/opt/bound.h \
	include/uni/types/opt/common.h \
	include/uni/types/opt/complexf.h \
	include/uni/types/opt/complexi.h \
	include/uni/types/opt/float.h \
	include/uni/types/opt/int.h \
	include/uni/types/opt/point.h \
	include/uni/types/opt/quant.h \
	include/uni/types/opt/range.h \
	include/uni/types/opt/vecf.h \
	include/uni/types/opt/veci.h \
	include/uni/types/opt.h \
	include/uni/types/options.h \
	include/uni/types/point.h \
	include/uni/types/quant.h \
	include/uni/types/range.h \
	include/uni/types/vec.h \
	include/uni/types/vecf.h \
	include/uni/types/veci.h \
	include/uni/decl.h \
	include/uni/ver.h
PRVHFILES :=

# test suite sources
TES_CFILES    :=
TES_CPPFILES  :=
TES_PUBHFILES :=
TES_PRVHFILES :=

# this defines all our usual targets
include $(AQ)/lib/slick/targets.mk
