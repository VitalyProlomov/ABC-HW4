# makefile for task.asm
task: main.o input.o inrnd.o output.o real.o sort.o
	gcc -g -o task main.o input.o inrnd.o output.o real.o sort.o -no-pie
main.o: main.asm macros.mac
	nasm -f elf64 -g -F dwarf main.asm -l main.lst
input.o: input.asm
	nasm -f elf64 -g -F dwarf input.asm -l input.lst
inrnd.o: inrnd.asm
	nasm -f elf64 -g -F dwarf inrnd.asm -l inrnd.lst
output.o: output.asm
	nasm -f elf64 -g -F dwarf output.asm -l output.lst
real.o: real.asm
	nasm -f elf64 -g -F dwarf real.asm -l real.lst
sort.o: sort.asm
	nasm -f elf64 -g -F dwarf sort.asm -l sort.lst