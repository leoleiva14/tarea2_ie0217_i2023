CC = g++
CFLAGS = -Wall -std=c++11
EXECUTABLE = Diosito1

# Especifica los archivos fuente de tu proyecto
SOURCES = main.cpp 

# Genera una lista de archivos objeto para compilar
OBJECTS = $(SOURCES:.cpp=.o)

all: $(EXECUTABLE)

$(EXECUTABLE): $(OBJECTS)
	$(CC) $(CFLAGS) $(OBJECTS) -o $@

%.o: %.cpp
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJECTS) $(EXECUTABLE)

