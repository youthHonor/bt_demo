cmake_minimum_required(VERSION 3.10.2)

project(hello_BT)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(behaviortree_cpp)
find_package(Threads)
add_executable(${PROJECT_NAME} main.cpp)
target_link_libraries(${PROJECT_NAME} ${behaviortree_cpp_TARGETS})
#target_link_libraries(${PROJECT_NAME} BT::behaviortree_cpp)

