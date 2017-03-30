
NAME=blog
CCC=g++
AR=ar
DEPS=$(NAME).hh ../../inc/h/interlecto.hh ../../inc/l/interlecto.a
CFLAGS=-std=gnu++11 -fPIC -shared
OFLAGS=-std=gnu++11 -c
AFLAGS=rvs

all: $(NAME).so

$(NAME).so: $(NAME).cc $(DEPS)
	$(CC) -o $@ $< ../../inc/l/interlecto.a $(CFLAGS)

%.o: %.cc $(DEPS)
	$(CC) -o $@ $< $(OFLAGS)
