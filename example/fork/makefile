#ref https://www.gnu.org/software/make/manual/html_node/Wildcard-Function.html
CC=gcc
CFLAGS=-Wall
LDFLAGS=
SOURCES=$(wildcard *.c)
OBJECTS=$(patsubst %.c,%.o,$(wildcard *.c))
EXECUTABLE=$(notdir  ,$(CURDIR))

all: $(EXECUTABLE)
    
$(EXECUTABLE): $(SOURCES) 
	$(CC) $(CFLAGS) $(LDFLAGS) $(SOURCES) -o $(EXECUTABLE).o
	./$(EXECUTABLE).o

clean:
	rm -f *.o

