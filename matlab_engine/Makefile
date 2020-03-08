CC = g++
CFLAGS = -std=c++11
INCLUDE = -I/Applications/MATLAB_R2019b.app/extern/include/ -I/Applications/MATLAB_R2019b.app/simulink/include
LIB1 = /Applications/MATLAB_R2019b.app/bin/maci64
LIB2 = /Applications/MATLAB_R2019b.app/extern/bin/maci64

object_file = engdemo.o

engdemo	:	$(object_file)
	$(CC) $(CFLAGS) $(object_file) -o engdemo -I$(INCLUDE) -L$(LIB1) -L$(LIB2) -lmx -lmex -lmat -leng -lMatlabDataArray -lMatlabEngine

engdemo.o	:	engdemo.cpp
	$(CC) -c engdemo.cpp -o engdemo.o $(INCLUDE)

clean	:
	rm $(object_file) engdemo
