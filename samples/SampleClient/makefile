CXX = g++
CXXFLAGS = -I../../include -I/home/yohan/Documents/mavlink/generated/include/mavlink/v2.0/common -I/home/yohan/Downloads/NatNet_SDK/include
LIB_DIRS = -L/home/yohan/Downloads/NatNet_SDK/lib
LIBS = -lNatNet -lserial

SRCS = SampleClient_MavSender.cpp
OBJS = $(SRCS:.cpp=.o)

TARGET = build/SampleClient_MavSender

all: $(TARGET)

$(TARGET): $(OBJS)
	$(CXX) $(CXXFLAGS) -o $@ $^ $(LIB_DIRS) $(LIBS)

clean:
	rm -f $(OBJS) $(TARGET)

