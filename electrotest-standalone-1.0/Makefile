#utkast till Makefile

PREFIX=/usr/local

all: src/electrotest-standalone

src/electrotest-standalone: src/electrotest-standalone.c
	$echo "CFLAGS=$(CFLAGS)" | \
		fold -s -w 70 | \
		sed -e 's/^/# /'
	$(CC) $(CPPFLAGS) $(CFLAGS) $(LDCFLAGS) -o $@ $^ -lm

install: src/electrotest-standalone
	install -D src/electrotest-standalone \
		$(DESTDIR)$(PREFIX)/bin/electrotest-standalone
clean:
	rm -f src/electrotest-standalone

distclean: clean

uninstall:
	rm -f $(DESTDIR)$(PREFIX)/bin/electrotest-standalone

.PHONY: all install clean distclean uninstall
