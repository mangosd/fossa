PROG = coap_server
SOURCES = $(PROG).c ../../fossa.c
CFLAGS = -W -Wall -I../.. $(CFLAGS_EXTRA) -DNS_ENABLE_COAP

all: $(PROG)

$(PROG): $(SOURCES)
	$(CC) $(SOURCES) -o $@ $(CFLAGS)

$(PROG).exe: $(SOURCES)
	cl $(SOURCES) /I../.. /MD /Fe$@

clean:
	rm -rf *.gc* *.dSYM *.exe *.obj *.o a.out $(PROG)
