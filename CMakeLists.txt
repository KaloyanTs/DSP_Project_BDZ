cmake_minimum_required(VERSION 3.0.0)
project(BDZ VERSION 0.1.0)

include(CTest)
enable_testing()

add_executable(BDZ main.cpp BDZInterface.cpp Box.cpp CityMap.cpp Graph.cpp TrainMap.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
