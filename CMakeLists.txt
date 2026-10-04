cmake_minimum_required(VERSION 3.10)

project(MY3DGame CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(MyGame main.cpp
    olcPixelGameEngine.h)

target_link_libraries(MyGame 
                    user32 
                    gdi32 
                    opengl32 
                    gdiplus 
                    Shlwapi 
                    dwmapi ) 