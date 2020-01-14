JAVA = java
JAVAC = javac
CPP_FlAGS = -Wall -g 
L_FLAGS = -lm
TARGET = PA2

OUT_FILE = out.txt
IN_FILE = books.txt

TAR_FILE = scraffe_PA2.tar.gz
ZIP_FILE = scraffe_PA2.zip


JAVA_SRCS := \
	$(wildcard *.java)

ARGS = \
	$(IN_FILE) $(OUT_FILE)

HDRS := \
	$(wildcard *.h)

all: build
	@echo "All Done!"

build: 
	$(JAVAC) $(JAVA_SRCS) $(JAVA_FLAGS) -o $(TARGET)

run:
	$(JAVA) $(TARGET) $(ARGS)

tar: 
	tar -czvf $(TAR_FILE) $(JAVA_SRCS) $(HDRS) makefile

zip:
	zip $(ZIP_FILE) $(JAVA_SRCS) $(HDRS) makefile

handin:
	handin $(TAR_FILE)

gdb:
	gdb ./$(TARGET)

valgrind:
	valgrind --leak-check=full -v --show-leak-kinds-all $(JAVA) $(TARGET) $(CPP_SRCS)

clean:
	rm -f $(TARGET)

cat:
	cat $(OUT_FILE)

git:
	git push -u origin master






















	