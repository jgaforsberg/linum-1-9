#utkast till Makefile
CC=gcc

PREFIX=/usr/local

BIN=electrotest-standalone

all: src/electrotest-standalone

src/electrotest-standalone: src/electrotest-standalone.c
	$echo "CFLAGS=$(CFLAGS)" | \
		fold -s -w 70 | \
		sed -e 's/^/# /'
	$(CC) $(CFLAGS) -o $@ $^ -lm

clean:
	rm -f src/electrotest-standalone

install: src/electrotest-standalone
	install -D src/electrotest-standalone \
		$(DESTDIR)$(PREFIX)/bin/electrotest-standalone

uninstall:
	rm -f $(DESTDIR)$(PREFIX)/bin/electrotest-standalone

.PHONY: all install clean uninstall
