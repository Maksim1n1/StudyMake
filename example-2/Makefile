.PHONY: all debug release clean

RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS   = -g -O0 -Wall
RELEASE_EXEC  = hello
DEBUG_EXEC    = hello-dbg
S         = hello.cpp

all: debug release

debug: $(DEBUG_EXEC)

hello-dbg: $(S)
    g++ $(DEBUG_FLAGS) $(S) -o $(DEBUG_EXEC) 

release: $(RELEASE_EXEC)

hello: $(S)
    g++ $(RELEASE_FLAGS) $(S) -o $(RELEASE_EXEC)

clean:
    rm -f $(RELEASE_EXEC) $(DEBUG_EXEC)
