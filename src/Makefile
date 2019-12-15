prefix=/usr/local

mciso: mciso.c ciso.h
	$(CC) -static mciso.c -o mciso -lz

install: mciso
	install -m 0755 mciso $(prefix)/bin/mciso
