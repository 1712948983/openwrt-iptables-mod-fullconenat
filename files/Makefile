%.so: %.o
	$(CC) -shared -lxtables -o $@ $^
%.o: %.c
	$(CC) ${CFLAGS} -fPIC -D_INIT=$*_init -c -o $@ $<

all: libipt_FULLCONENAT.so libip6t_FULLCONENAT.so

