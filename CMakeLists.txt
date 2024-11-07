cmake_minimum_required(VERSION 3.27.0)
project(linuxcdemo VERSION 1.0 LANGUAGES C)

# specify the C standard
set(CMAKE_CXX_STANDARD C99)
set(CMAKE_C_STANDARD_REQUIRED True)
# set output executable file directory
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

include_directories("./includes/")

add_executable(linuxcdemo "./src/main.c")
