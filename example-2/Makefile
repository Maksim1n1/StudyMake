.PHONY: all debug release clean

RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS   = -g -O0 -Wall
RELEASE_EXEC  = Kazino-Royal
DEBUG_EXEC    = Kazino-Royal-dbg
SRC         = Kazino-Royal.cpp

all: debug release

debug: $(DEBUG_EXEC)

Kazino-Royal-dbg: $(SRC)
	g++ $(DEBUG_FLAGS) $(SRC) -o $(DEBUG_EXEC) 

release: $(RELEASE_EXEC)

Kazino-Royal: $(SRC)
	g++ $(RELEASE_FLAGS) $(SRC) -o $(RELEASE_EXEC)

clean:
	rm -f $(RELEASE_EXEC) $(DEBUG_EXEC)
