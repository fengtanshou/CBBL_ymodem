include ../Makefile.common

OBJS+=startup.o
OBJS+=common.o
OBJS+=download.o
OBJS+=stm32f10x_it.o
OBJS+=system_stm32f10x.o
OBJS+=upload.o
OBJS+=ymodem.o
OBJS+=main.o
#OBJS+=*.o
 
all: src

src: app.a

app.a: $(OBJS)
	$(AR) cr app.a $(OBJS)

.PHONY: src clean
clean:
	rm -f app.a $(OBJS)
