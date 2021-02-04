CC = gcc
L_FLAGS = -lm
CFLAGS = -Wall -g -save-temps
TARGET = 

OUT_FILE = 
IN_FILE =

TAR_FILE = scraffe.tar.gz
TAR_EXTRAS = 
ZIP_FILE = scraffe.zip


C_SRCS := \
	$(wildcard *.c)

ARGS = \
	$(IN_FILE)

HDRS := \
	$(wildcard *.h)

CTEMPS := \
	$(wildcard *.i) $(wildcard *.o) $(wildcard *.s)

all: build
	@echo "All Done!"

build: 
	$(CC) $(CFLAGS) -save-temps $(C_SRCS) -o $(TARGET)

run:
	./$(TARGET) $(ARGS)

tar: 
	tar -czvf $(TAR_FILE) $(C_SRCS) $(HDRS) $(TAR_EXTRAS) makefile

untar: 
	tar -zxvf $(TAR_FILE)

zip:
	zip $(ZIP_FILE) $(C_SRCS) $(HDRS) makefile

unzip:
	unzip $(ZIP_FILE)

handin:
	handin $(TAR_FILE)

gdb:
	gdb ./$(TARGET)

valgrind:
	valgrind --leak-check=full -v --show-leak-kinds-all ./$(TARGET) $(C_SRCS)

clean:
	rm -f $(TARGET) $(CTEMPS)

cat:
	cat $(OUT_FILE)

git:
	git push -u origin master






















	
