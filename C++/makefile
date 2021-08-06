CPP = g++
CPP_FlAGS = -Wall -g -std=c++11
L_FLAGS = -lm
TARGET = 

OUT_FILE = 
IN_FILE = 

TAR_FILE = .tar.gz
ZIP_FILE = .zip


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

untar: 
	tar -zxvf $(TAR_FILE) $(CPP_SRCS) $(HDRS) makefile

zip:
	zip $(ZIP_FILE) $(CPP_SRCS) $(HDRS) makefile

unzip:
	unzip $(ZIP_FILE)

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
	git push -u origin main






















	
