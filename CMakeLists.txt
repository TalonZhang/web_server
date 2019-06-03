cmake_minimum_required(VERSION 3.13)
project(web_server)

set(CMAKE_CXX_STANDARD 14)

add_executable(web_server main.cpp)

find_package(Threads REQUIRED)
target_link_libraries(web_server Threads::Threads)