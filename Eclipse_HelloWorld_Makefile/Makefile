BUILD_TIME := $(shell date +%Y%h%d_%H:%M:%S)

CXXFLAGS =	-O2 -g -Wall -fmessage-length=0 -D __BUILD_TIME=\"$(BUILD_TIME)\"

OBJS =		HelloWorld.o

LIBS =

TARGET =	HelloWorld

$(TARGET):	$(OBJS)
	@echo Build $(BUILD_TIME) started.
	$(CXX) -o $(TARGET) $(OBJS) $(LIBS)
	@echo Build $(BUILD_TIME) finished.

all:	$(TARGET)

clean:
	rm -f $(OBJS) $(TARGET)
