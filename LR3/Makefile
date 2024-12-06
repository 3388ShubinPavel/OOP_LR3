CXX = g++
CXXFLAGS = -c -Wall -std=c++17

SRCS = main.cpp segment.cpp ship.cpp shipmanager.cpp cell.cpp gamefield.cpp scanner.cpp doubledamage.cpp bombardment.cpp abilitymanager.cpp game.cpp gamestate.cpp
OBJS = $(SRCS:.cpp=.o)

HEADERS = segment.h ship.h shipmanager.h cell.h gamefield.h scanner.h doubledamage.h bombardment.h abilitymanager.h ability.h infoholder.h game.h gamestate.h

TARGET = game

all: $(TARGET)

$(TARGET): $(OBJS)
	$(CXX) $(OBJS) -o $(TARGET) && make clean

%.o: %.cpp %.h
	$(CXX) $(CXXFLAGS) $<

main.o: main.cpp
	$(CXX) $(CXXFLAGS) main.cpp

clean:
	del *.o $(TARGET)

