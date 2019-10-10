#Akshobh Mirapurkar 
#HW5, Makefile 
#September 25th, 2019

CC=g++

CFLAGS=-c -Wall

REMOVE=rm

all: build archive

build: main.o game.o othello.o 
	$(CC) main.o game.o othello.o -o game

main.o: main.cc 
	$(CC) $(CFLAGS) main.cc 

game.o: game.cc
	$(CC) $(CFLAGS) game.cc

othello.o: othello.cc
	$(CC) $(CFLAGS) othello.cc

#make a tarball of the current directory and call it game.tar
archive: 
	tar cvzf game.tgz *

clean:
	$(REMOVE) -rf *o game
	$(REMOVE) -rf *tgz game