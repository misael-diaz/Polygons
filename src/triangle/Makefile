#!/usr/bin/make
#
# Polygons					February 11, 2024
#
# source: src/triangle/Makefile
# author: @misael-diaz
#
# Synopsis:
# Defines the Makefile for building the program with GNU make.
#
# Copyright (c) 2024 Misael Díaz-Maldonado
# This file is released under the GNU General Public License as published
# by the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
#

include make-inc

all: $(TRIANGLE_BIN)

$(TRIANGLE_BIN): $(TRIANGLE_OBJ)
	$(CXX) $(CXXOPT) $(TRIANGLE_OBJ) -o $(TRIANGLE_BIN)

$(TRIANGLE_OBJ): $(HEADERS) $(TRIANGLE_CXX)
	$(CXX) $(INC) $(CXXOPT) -c $(TRIANGLE_CXX) -o $(TRIANGLE_OBJ)

clean:
	/bin/rm -f *.obj *.bin
