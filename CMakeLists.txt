cmake_minimum_required(VERSION 3.27.0)
project(linuxcdemo VERSION 1.0 LANGUAGES C)

# specify the C standard
set(CMAKE_C_STANDARD 99)
set(CMAKE_C_STANDARD_REQUIRED TRUE)
# set output executable file directory
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

include_directories("./includes/")

set(MY_EXECUTABLE_NAME "linuxcdemo")

add_executable(
  ${MY_EXECUTABLE_NAME}
  "./src/main.c"
)
