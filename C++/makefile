CPP = g++
CPP_FlAGS = -Wall -g -std=c++11
L_FLAGS = -lm
TARGET = PA2

OUT_FILE = out.txt
IN_FILE = books.txt

TAR_FILE = scraffe_PA2.tar.gz
ZIP_FILE = scraffe_PA2.zip


CPP_SRCS := \
	$(wildcard *.cpp)

ARGS = \
	$(IN_FILE) $(OUT_FILE)

HDRS := \
	$(wildcard *.h)

all: build
	@echo "All Done!"

build: 
	$(CPP) $(CPP_SRCS) $(CPP_FLAGS) -std=c++11 -o $(TARGET)

run:
	./$(TARGET) $(ARGS)

tar: 
	tar -czvf $(TAR_FILE) $(CPP_SRCS) $(HDRS) makefile

zip:
	zip $(ZIP_FILE) $(CPP_SRCS) $(HDRS) makefile

handin:
	handin $(TAR_FILE)

gdb:
	gdb ./$(TARGET)

valgrind:
	valgrind --leak-check=full -v --show-leak-kinds-all ./$(TARGET) $(CPP_SRCS)

clean:
	rm -f $(TARGET)

cat:
	cat $(OUT_FILE)

git:
	git push -u origin master






















	
