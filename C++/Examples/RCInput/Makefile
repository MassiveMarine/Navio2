CXX ?= g++
NAVIO = ../../Navio

PIGPIO_PATH ?= $(NAVIO)/pigpio

LIB = -L$(PIGPIO_PATH)

INCLUDES = -I ../../Navio -I$(PIGPIO_PATH)

all:
	$(MAKE) -C ../../Navio all
	$(CXX) -std=gnu++11 $(INCLUDES) $(LIB) RCInput.cpp -L$(NAVIO) -lnavio -o RCInput -lrt -lpthread -lpigpio

clean:
	rm -f RCInput

