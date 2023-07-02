# Directories
S_DIR = .
B_DIR = ./bin

# Files
S_FILES = $(S_DIR)/main.cpp
#D_FILES = $(S_DIR)/lib/*

# Output
EXEC = $(B_DIR)/gdcpp

# Build settings
CC = g++
CC_FLAGS = -g -Wall 

# SDL options
CC_SDL= #-lSDL2 -lSDL2_image -lSDL2_mixer -lSDL2_ttf #-ludev # I am pretty sure this isn't necessary but keep in file just in case

#$(D_FILES)

default: build

build: #./include/*
	$(CC) $(CC_FLAGS) $(S_FILES) -o $(EXEC) $(CC_SDL)

run: build
	$(EXEC)

debugger: build
	gdb $(EXEC)

clean:
	rm -rf $(B_DIR)/*
