cmake_minimum_required(VERSION 3.27)
project(DrogonMyWebServer)

set(CMAKE_CXX_STANDARD 23)

add_executable(DrogonMyWebServer main.cpp
        controller/testctrl.cc)

find_package(Drogon CONFIG REQUIRED)
target_link_libraries(DrogonMyWebServer PRIVATE Drogon::Drogon)