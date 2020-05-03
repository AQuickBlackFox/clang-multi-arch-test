CLANG_X86_BIN_DIR=~/llvm11_x86_64/bin
CLANG_ARM_BIN_DIR=~/llvm11_arm/bin
CLANG_AARCH64_BIN_DIR=~/llvm11_aarch64/bin

GNU_X86_CC=gcc
GNU_X86_CXX=g++
CLANG_X86_CC=clang
CLANG_X86_CXX=clang++

GNU_ARM_CC=arm-linux-gnueabihf-gcc
GNU_ARM_CXX=arm-linux-gnueabihf-g++
GNU_ARM

GNU_AARCH64_CC=
GNU_AARCH64_CXX

CCFLAGS=-I../include -I./include
CXXFLAGS=-I../include -I./include -std=c++14


all: clang-multi-arch-test

clang-multi-arch-test: clang-multi-arch-test.cpp
	mkdir -p bin
	$(CXX) $(CXXFLAGS) $^ -o ./bin/$@
clean:
	rm -rf bin
  
