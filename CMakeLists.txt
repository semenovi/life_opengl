cmake_minimum_required (VERSION 2.6)
project(life)
set(LIFE_SRC_LIST src/main.cpp)
add_executable(life ${LIFE_SRC_LIST})
add_subdirectory(include)
target_link_libraries(life life_lib)
target_link_libraries(life opengl32)
target_link_libraries(life glu32)
set(CMAKE_CONFIGURATION_TYPES "Debug;Release" CACHE STRING "Configs" FORCE)