cmake_minimum_required(VERSION 3.27)
project(movie_app)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)


find_package(Qt5 COMPONENTS
        Core
        Gui
        Widgets
        REQUIRED)

add_executable(movie_app main.cpp)
target_link_libraries(movie_app
        Qt5::Core
        Qt5::Gui
        Qt5::Widgets
)

