OBJS =  main.o type_lexeme.o core_env.o kernel_mem.o kernel_sysdep.o

.c.o :
	gcc -c -Wall  -Wundef -Wpointer-arith -Wshadow -Wcast-qual \
	    -Wcast-align -Winline -Wmissing-declarations -Wredundant-decls \
	    -Wmissing-prototypes -Wnested-externs \
	    -Wstrict-prototypes -Waggregate-return -Wno-implicit $<

vander : $(OBJS) 
	gcc -o mingvs $(OBJS) -lm -ltermcap

# Dependencies generated using "gcc -MM *.c"
