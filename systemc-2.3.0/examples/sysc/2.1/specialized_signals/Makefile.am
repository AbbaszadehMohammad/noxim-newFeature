## ****************************************************************************
##
##  Licensed to Accellera Systems Initiative Inc. (Accellera) under one or
##  more contributor license agreements.  See the NOTICE file distributed
##  with this work for additional information regarding copyright ownership.
##  Accellera licenses this file to you under the Apache License, Version 2.0
##  (the "License"); you may not use this file except in compliance with the
##  License.  You may obtain a copy of the License at
##
##   http://www.apache.org/licenses/LICENSE-2.0
##
##  Unless required by applicable law or agreed to in writing, software
##  distributed under the License is distributed on an "AS IS" BASIS,
##  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
##  implied.  See the License for the specific language governing
##  permissions and limitations under the License.
##
## ****************************************************************************
##
##  examples/sysc/2.1/specialized_signals/Makefile.am --
##  Process this file with automake to produce a Makefile.in file.
##
##  Original Author: Andy Goodrich, Forte Design Systems, 17 June 2003
##
## ****************************************************************************
##
##  MODIFICATION LOG - modifiers, enter your name, affiliation and
##  changes you are making here:
##
##  Modifier Name & Affiliation:
##  Description of Modification:
##
## ****************************************************************************

include $(top_srcdir)/config/Make-rules.examples

CXX_FILES = \
	main.cpp \
	scx_signal_int.cpp \
	scx_signal_uint.cpp \
	scx_signal_signed.cpp \
	scx_signal_unsigned.cpp 

H_FILES = \
	scx_signal_int.h \
	scx_signal_uint.h \
	scx_signal_signed.h \
	scx_signal_unsigned.h 

check_PROGRAMS = specialized_signals
TESTS = $(check_PROGRAMS) 

specialized_signals_SOURCES = $(CXX_FILES) $(H_FILES)

specialized_signals_LDADD = -L$(prefix)/lib-$(TARGET_ARCH) -lsystemc -lm

specialized_signals_INSTALLS = $(specialized_signals_SOURCES) 


all:
	@echo "To compile and run this example type"
	@echo "   make check "

install-data-local:
	@$(NORMAL_INSTALL)
	$(mkinstalldirs) .
	for file in $(specialized_signals_INSTALLS); do \
		$(INSTALL_DATA) $(srcdir)/$$file ./$$file; \
	done



uninstall-local:
	@$(NORMAL_UNINSTALL)
	for file in $(specialized_signals_INSTALLS); do \
		rm -f ./$$file; \
	done

## Taf!
