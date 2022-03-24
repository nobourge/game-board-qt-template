cmake_minimum_required(VERSION 3.21)
project(game-board-qt-template)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_PREFIX_PATH "~/Qt/6.2.4/gcc_64/lib/cmake")

include_directories(.)
find_package(Qt6 CONFIG REQUIRED COMPONENTS Widgets)

add_executable(game-board-qt-template
        qt_main.cpp
        qt_main.h canvas.cpp canvas.h)


target_link_libraries(game-board-qt-template Qt6::Widgets)