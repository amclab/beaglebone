CFLAGS = -mcpu=cortex-a8 -g
OPTIMIZATION_FLAGS= -O2


all: clean bin

compile: code.c startup.s
	$(CC)gcc $(CFLAGS) $(OPTIMIZATION_FLAGS) -c code.c -o code.o
	$(CC)as $(CFLAGS) startup.s -o startup.o

link: compile
	$(CC)ld -T linker.lds code.o startup.o -o code.elf

bin: link
	$(CC)objcopy --gap-fill=0xff -O binary code.elf code.bin


clean:
	rm -f startup.o
	rm -f code.o code.elf code.bin *~
