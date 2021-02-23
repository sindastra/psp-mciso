prefix ?= /usr/local
CC ?= gcc

all: mciso

mciso: mciso.c ciso.h
	$(CC) $(CFLAGS) -static mciso.c -o mciso -lz

install: mciso
	install -m 0755 mciso $(prefix)/bin/mciso
	install -m 0644 mciso.1 $(prefix)/share/man/man1/mciso.1
