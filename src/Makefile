
TESTDIR=./tests/from_MagAOX

all: flatlogcodes

flatlogcodes: flatlogcodes.cpp
	g++ -o flatlogcodes flatlogcodes.cpp

test: flatlogcodes
	@( cd $(TESTDIR)/ && make test )

install: all
	mkdir -p ../bin
	install flatlogcodes ../bin

.PHONY: clean
clean:
	rm -f flatlogcodes
	rm -f *.o
