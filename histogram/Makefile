#----- Modify CC and CFLAGS as appropriate in your environment
CC = gcc
CFLAGS = -O3 -fopenmp

LIB = -lm -lc

UNITFILES = 

#------------ EXECUTABLE FILES ---------------

histo : histo.o $(UNITFILES)
	$(CC) $(CFLAGS) -o histo histo.o $(UNITFILES) $(LIB)

histo_locks : histo_locks.o $(UNITFILES)
	$(CC) $(CFLAGS) -o histo_locks histo_locks.o $(UNITFILES) $(LIB)

clean:
	rm -f histo histo_locks *.o

histo.o : histo.c
	$(CC) $(CFLAGS) -c histo.c $(INCLUDE) 

histo_locks.o : histo_locks.c
	$(CC) $(CFLAGS) -c histo_locks.c $(INCLUDE) 
