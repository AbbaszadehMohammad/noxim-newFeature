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
##  examples/sysc/Makefile.am --
##  Process this file with automake to produce a Makefile.in file.
##
##  Original Author: Martin Janssen, Synopsys, Inc.
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

SUBDIRS = \
	fft_flpt \
	fft_fxpt 


EXAMPLES_DIR = $(prefix)/examples/sysc/fft

install-data-local:
	@$(NORMAL_INSTALL)
	$(mkinstalldirs) $(EXAMPLES_DIR)

uninstall-local:
	@$(NORMAL_UNINSTALL)
	-rmdir $(EXAMPLES_DIR)

## Taf!
