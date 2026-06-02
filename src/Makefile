FC = gfortran -g -static-libgfortran
SOURCE = dungeon.o game.o gdt.o objects.o parser.o rooms.o subr.o timefnc.o verbs.o
EXE = dungeon
.PHONY: clean

all : dungeon

dist : dungeon
	strip $(EXE)

clean :
	rm -f *.o dungeon

dungeon : $(SOURCE)
	$(FC) -o $(EXE) $^ 

