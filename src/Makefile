CC= g++-4.9
CFLAGS=-std=c++11 -g -O2
LDFLAGS=
SOURCES=distTest.cpp
OBJECTS=$(SOURCES:.cpp=.o)
EXECUTABLE=test

all: clean $(SOURCES) $(EXECUTABLE)

$(EXECUTABLE): $(OBJECTS)
	$(CC) $(LDFLAGS) $(OBJECTS) -o $@

%.o: %.cpp
	$(CC) $(CFLAGS) $< -c

clean:
	$(RM) count *.o *~

