JAVA = java
JAVAC = javac
CPP_FlAGS = -Wall -g 
L_FLAGS = -l
TARGET = 

FILEPATH := \
	$(wildcard *.java) \
	$(wildcard */*.java) \
	$(wildcard */**/*.java)

RUNPATH := \
	$(wildcard *.java) \
	$(wildcard */*.java) \
	$(wildcard */**/*.java)

CLEANPATH = $(RUNPATH)

TAR_FILE = scraffe_.tar.gz
ZIP_FILE = scraffe_.zip
OUT_FILE = 
IN_FILE = 

ARGS = \
	$(IN_FILE) $(OUT_FILE)

default: $(FILEPATH)
	$(JAVAC) $(FILEPATH)

run: $(RUNPATH)
	$(JAVA) $(TARGET) 

tar: 
	tar -czvf $(TAR_FILE) $(JAVA_SRCS) makefile

untar:
	tar -xzvf $(TAR_FILE)

zip:
	zip $(ZIP_FILE) -r $(JAVA_SRCS) makefile

handin:
	handin $(TAR_FILE)

valgrind:
	valgrind --leak-check=full -v --show-leak-kinds-all $(JAVA) $(TARGET)

clean:
	rm -f $(CLEANPATH)

cat:
	cat $(OUT_FILE)

git:
	git push -u origin master






















	
