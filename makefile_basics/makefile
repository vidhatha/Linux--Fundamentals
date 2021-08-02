# Usage:
# make		# compile all binaries
# make clean	# remove all binaries and objects

.PHONY = all clean

cc = gcc	# compiler to use

LINKERFLAG = -lm

SRCS := foo.c
BINS := foo

all: foo

foo: foo.o
	@echo "Linking binary.."
	gcc -lm foo.o -o foo

foo.o: foo.c
	@echo "Compiling binary.."
	gcc -c foo.c

clean:
	@echo "Cleaning up .."
	rm -rvf foo.o foo
