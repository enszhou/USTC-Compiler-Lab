sample.out: sample.o
	gcc sample.o -o sample.out

sample.o: sample.s
	gcc -c sample.s -o sample.o

sample.s: sample.i
	gcc -S sample.i -o sample.s
	gcc -S sample.c -o sample_32.s

sample.i: sample.c
	gcc -E sample.c -o sample.i