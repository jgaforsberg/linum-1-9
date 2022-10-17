#utkast till Makefile
CC=gcc

BININST=/usr/bin

BIN=electrotest-standalone

all: electrotest-standalone

electrotest-standalone: electrotest-standalone.o
	$(CC) -fpic -o $@ electrotest-standalone.o -lm

electrotest-standalone.o: electrotest-standalone.c
	$(CC) -c -fpic electrotest-standalone.c

clean:
	rm -rf *.o electrotest-standalone

install:
	sudo cp $(BIN) $(BININST)

uninstall:
	sudo rm -rf $(BININST)/$(BIN)

