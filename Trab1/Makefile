CXXFLAGS=$(shell pkg-config --cflags gtk+-3.0)
CXXFLAGS+= -std=c++11 -O2 -Wall -Wextra -Wno-unused-parameter -rdynamic
LDFLAGS=$(shell pkg-config --libs gtk+-3.0)

all: $(basename $(wildcard *.cpp))

debug: CXXFLAGS += -g
debug: all

clean:
	@rm $(basename $(wildcard *.cpp))
