cmake_minimum_required(VERSION 3.0)
project(laboratories)

set(CMAKE_CXX_STANDARD 17)

find_package(SFML
        COMPONENTS
        system window graphics network audio REQUIRED
        )

add_executable(laboratories main.cpp first_semester/1/1.cpp first_semester/2/2.cpp first_semester/3/3.cpp first_semester/4/4.cpp first_semester/5/5.cpp first_semester/6/6.cpp first_semester/6/io/input.cpp first_semester/6/io/output.cpp first_semester/9/9.cpp first_semester/10/10.cpp first_semester/8/8.cpp first_semester/11/11.cpp second_semester/1/1.cpp second_semester/2/String.cpp second_semester/3/Complex.cpp  second_semester/5/Vector.cpp second_semester/6/Logger.cpp second_semester/6/Config/Config.cpp second_semester/7/shape/Shape.cpp second_semester/7/shape/triange/Triangle.cpp second_semester/7/shape/circle/Circle.cpp second_semester/7/shape/square/Rectangle.cpp second_semester/4/Matrix.cpp)

target_link_libraries(laboratories sfml-graphics sfml-audio)
