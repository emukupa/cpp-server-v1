cmake_minimum_required(VERSION 3.10.2)
project(initiate_site)

set(CMAKE_CXX_STANDARD 17)
set(THREADS_PREFER_PTHREAD ON)

find_package(Boost COMPONENTS system filesystem REQUIRED)
find_package(Threads)

include_directories(${Boost_INCLUDE_DIRS})
add_executable(initiate_site main.cpp)
target_link_libraries(initiate_site ${Boost_LIBRARIES} Threads::Threads)




