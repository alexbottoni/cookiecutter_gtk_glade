# change application name here (executable output name)
TARGET={{cookiecutter.main_c_source_filename}}

# compiler
CC=gcc
# debug
DEBUG=-g
# optimisation
OPT=-O0
# warnings
WARN=-Wall

PTHREAD=-pthread

CCFLAGS=$(DEBUG) $(OPT) $(WARN) $(PTHREAD) -pipe

GTKLIB=`pkg-config --cflags --libs gtk+-3.0`

# linker
LD=gcc
LDFLAGS=$(PTHREAD) $(GTKLIB) -export-dynamic

OBJS=	{{cookiecutter.main_c_source_filename}}.o

all: $(OBJS)
	$(LD) -o $(TARGET) $(OBJS) $(LDFLAGS)
	
main.o: src/{{cookiecutter.main_c_source_filename}}.c
	$(CC) -c $(CCFLAGS) src/{{cookiecutter.main_c_source_filename}}.c $(GTKLIB) -o {{cookiecutter.main_c_source_filename}}.o
	
clean:
	rm -f *.o $(TARGET)