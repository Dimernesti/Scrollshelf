cmake_minimum_required(VERSION 3.8)
project(Scrollshelf)

set(CMAKE_CXX_STANDARD 17)

set(SOURCE_FILES src/main.cpp)
find_package(Qt5Core REQUIRED)
find_package(Qt5Sql REQUIRED)
add_executable(${PROJECT_NAME} ${SOURCE_FILES})
target_link_libraries(${PROJECT_NAME} Qt5::Core Qt5::Sql)
