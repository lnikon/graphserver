cmake_minimum_required(VERSION 3.5.0)

project(graph_server)

find_package(Poco REQUIRED Net Util)

add_executable(exec_me main.cpp)

target_link_libraries(exec_me PUBLIC Poco::Net Poco::Util)