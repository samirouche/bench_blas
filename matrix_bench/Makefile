
PROG = bench
CC = g++
CPPFLAGS = -g -Wall
OBJS = matrix.o main_bench.o
LIBS = -lblas

$(PROG): $(OBJS)
		$(CC) $(CPPFLAGS)  matrix.o main_bench.o  -o $(PROG) $(LIBS)
matrix.o: matrix.h
		$(CC) $(CPPFLAGS) -c matrix.cpp

main_bench.o:
	 	$(CC) $(CPPFLAGS) -c main_bench.cpp

clean:
		rm -f core $(PROG) $(OBJS)
