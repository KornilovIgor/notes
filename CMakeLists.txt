#/src - source files (*.cpp) 
#/include - headers files (*.h)
#CMakeLists.txt - main CMake-file
#.gitignore



cmake_minimum_required(VERSION 3.22) #change version

set(PROJECT_NAME myProject) #change name
project(${PROJECT_NAME})

file(GLOB CPPS "src/*.cpp")

include_directories("${PROJECT_SOURCE_DIR}/include")

add_executable(${PROJECT_NAME} ${CPPS})
