CFLAGS=-std=c++11
CC=g++

all: stack-vm

stack-vm: stack-vm.o main.o
	$(CXX) $(CFLAGS) stack-vm.o main.o -o stack-vm

main.o: main.cpp
	$(CXX) $(CFLAGS) -c main.cpp main.o
stack-vm.o: stack-vm.h stack-vm.cpp
	$(CXX) $(CFLAGS) -c stack-vm.cpp

clean:
	rm -f *.o stack-vm
