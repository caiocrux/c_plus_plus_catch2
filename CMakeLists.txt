cmake_minimum_required(VERSION 3.14)

project(leilao)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_BUILD_TYPE Debug)

include_directories(include)
include_directories(src)
include_directories(tests)

file(GLOB leilao_SRC CONFIGURE_DEPENDS "./src/*.cpp")
file(GLOB leilao_INC CONFIGURE_DEPENDS "./include/*.hpp")

add_executable( ${PROJECT_NAME} ${leilao_INC} ${leilao_SRC})
