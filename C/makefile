CC = gcc
L_FLAGS = -lm
CFLAGS = -Wall -g -save-temps
TARGET = PA1

OUT_FILE = 
IN_FILE = 20 25

TAR_FILE = scraffe_PA1.tar.gz
TAR_EXTRAS = PA1.docx
ZIP_FILE = scraffe_PA1.zip


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






















	
