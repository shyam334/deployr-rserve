# Makefile for C++ Rserve clients.
#
# $Id: Makefile.in 213 2008-01-10 22:46:01Z urbanek $

SRC = $(wildcard *.cc)
OBJ = $(SRC:%.cc=%.o)
DST = demo1 rcons rsdown

LIBS+=-ldl -lcrypt 
CPPFLAGS+=-DHAVE_CONFIG_H

all: $(DST) $(OBJ)

%: Rconnection.o %.o
	$(CXX) $^ -o $@ $(LIBS)

debug:
	$(MAKE) CXXFLAGS=-g all

clean:
	rm -rf *~ *.o \#* .\#* $(DST)
