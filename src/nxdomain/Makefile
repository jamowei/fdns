all: nxdomain

include ../common.mk

%.o : %.c $(H_FILE_LIST)
	$(CC) $(CFLAGS) $(EXTRA_CFLAGS) $(INCLUDE) -c $< -o $@

nxdomain: $(OBJS)
	$(CC)  $(LDFLAGS) -o $@ $(OBJS)  $(LIBS) $(EXTRA_LDFLAGS)

clean:; rm -f *.o nxdoamain *.gcov *.gcda *.gcno

distclean: clean
