cc = gcc
CFLAGS = -Wall -Wextra -Wfatal-errors

all: program 

program: main.o isEven.o isOdd.o
	$(cc) $(CFLAGS) main.o isEven.o isOdd.o -o program

main.o: main.c 
	$(cc) $(CFLAGS) -c main.c -o $@

isEven.o: isEven.c 
	$(cc) $(CFLAGS) -c isEven.c -o $@

isOdd.o: isOdd.c 
	$(cc) $(CFLAGS) -c isOdd.c -o $@

clean:
	rm -f program main.o isEven.o isOdd.o