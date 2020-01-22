JAVA = java
JAVAC = javac
CPP_FlAGS = -Wall -g 
L_FLAGS = 
TARGET = 

OUT_FILE = 
IN_FILE = 

TAR_FILE = scraffe_PA2.tar.gz
ZIP_FILE = scraffe_PA2.zip

FILEPATH = 
RUNPATH = 

JAVA_SRCS := \
	$(wildcard *.java)

ARGS = \
	$(IN_FILE) $(OUT_FILE)

#HDRS := \
#	$(wildcard *.h)

all: build
	@echo "All Done!"

default: $(FILEPATH)$(JAVA_SRCS)
	$(JAVAC) $(FILEPATH)$(JAVA_SRCS) 

run: $(RUNPATH)$(JAVA_SRCS)
	$(JAVA) $(TARGET) 

tar: 
	tar -czvf $(TAR_FILE) $(JAVA_SRCS) $(HDRS) makefile

zip:
	zip $(ZIP_FILE) -r $(JAVA_SRCS) #$(HDRS) makefile

handin:
	handin $(TAR_FILE)

valgrind:
	valgrind --leak-check=full -v --show-leak-kinds-all $(JAVA) $(TARGET) $(CPP_SRCS)

clean:
	rm -f $(TARGET)

cat:
	cat $(OUT_FILE)

git:
	git push -u origin master






















	
