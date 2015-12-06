OBJS:=main.o
TARGET:=tamaserver
CFLAGS:=-ggdb

UNAME_S := $(shell uname -s)
ifneq ($(UNAME_S),Darwin)
    LDFLAGS:=-lrt
endif

$(TARGET): $(OBJS)
	$(CC) $(LDFLAGS) -o $@ $^

clean:
	rm -f $(OBJS) $(TARGET)

.PHONEY: clean
