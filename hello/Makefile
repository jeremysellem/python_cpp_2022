CPPFLAGS += -I /usr/local/Cellar/python@3.7/3.7.12_1/Frameworks/Python.framework/Versions/3.7/include/python3.7m -std=c++17
LIBS=/usr/local/Cellar/python@3.7/3.7.12_1/Frameworks/Python.framework/Versions/3.7/lib/libpython3.7m.dylib

COMPOSANT = hello_component

LIBSO = ${COMPOSANT}.so
LIBSO_OBJS = ${COMPOSANT}.o

include ../gcc.mk
include ../pybind11.mk


all: $(LIBSO)
clean:
	rm -f ${LIBSO}  ${LIBSO_OBJS}


${DESTINATION_LIBSO}: ${LIBSO}
	cp $< $@

