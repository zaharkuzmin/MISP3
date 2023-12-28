.PHONY: all clean test format

CXX=g++
OFLAGS=-O2 -Wall -DNDEBUG
LDFLAGS=-lUnitTest++ 

SOURCES=main.cpp modRoutingCipher.cpp
HEADERS=modRoutingCipher.h
EXECUTABLE=test2


$(EXECUTABLE): $(SOURCES)
	$(CXX)  $(SOURCES)  -o $(EXECUTABLE) $(OFLAGS) $(LDFLAGS)

test: $(EXECUTABLE)
	./$(EXECUTABLE) 

format:
	astyle $(SOURCES) $(HEADERS)
clean:
	rm -f $(EXECUTABLE) *.orig
