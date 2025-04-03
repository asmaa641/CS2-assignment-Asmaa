We will be making a calculator that includes several and we will use github to collaborate.
 We will also build the files using cmake and make and we will use version control

How to build:
1) To build using g++, write the following code in the terminal:
g++ -o out.exe  <list here ALL project source files>
in our case it will be: 
g++ -o calc test2.cpp calc.cpp  

And then run calc by doing
./calc

2) To build using cmake and make, first make a CMakeList.txt which will have the following:
cmake_minimum_required(VERSION 3.10)

project(CS2-assignment-Asmaa)

set(SOURCE_FILES 
    calc.cpp
    test2.cpp	   
)

add_executable(calc ${SOURCE_FILES})

Then,cmake to create the Makefile automatically. Then, run make to build the project and produce exe. Then run the exe by doing
./exename (in our case it is ./calc)

To use our library, open test2.cpp and use our different functions to add/subtract/divide/multiply/factorial/find gcd/lcm
generate random number in a range/do parsing for the bonus part for any numbers you'd like, then run make again.
