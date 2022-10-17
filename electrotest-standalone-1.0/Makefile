#utkast till Makefile
CC=gcc

PREFIX=/usr/bin

BIN=electrotest-standalone

all: src/electrotest-standalone

src/electrotest-standalone: src/electrotest-standalone.c
	$echo "CFLAGS=$(CFLAGS)" | \
		fold -s -w 70 | \
		sed -e 's/^/# /'
	$(CC) $(CFLAGS) -o $@ $^ -lm

clean:
	rm -f src/electrotest-standalone

install:
	sudo cp $(BIN) $(BININST)

uninstall:
	sudo rm -rf $(BININST)/$(BIN)

