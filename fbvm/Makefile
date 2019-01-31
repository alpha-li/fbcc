OBJS = fbvm.o
CFLAGS = -g -Wall -O2
LIBS =
LFLAGS	=

all: fbvm

clean:
	rm -f *.o *~ fbvm

fbvm.o: fbvm.c fbvmspec.h fbvminstr.h

fbvm: $(OBJS)
	gcc -g $(OBJS) $(LFLAGS) -o fbvm $(LIBS)

.c.o:
	gcc	$(CFLAGS) -c $*.c

